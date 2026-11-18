# IQ Wallet NFC · Laboratorio web

Maqueta **con lectura real Web NFC** y saldo de demostración guardado en `localStorage` del navegador. No manipula tarjetas, no retira dinero real, no tiene cuentas ni base de datos.

## Despliegue

Subir esta carpeta como `/nfc-wallet/` bajo la raíz pública del servidor HTTPS. Ejemplo: `https://tu-dominio.mx/nfc-wallet/`. Este repositorio contiene otras demos: **no reemplazar el `index.html` de la raíz**.

No necesita compilación ni PHP. La publicación debe usar un dominio con certificado HTTPS válido y la página debe abrirse directamente, no en un iframe.

## Prueba en Android

1. Activa NFC en Android.
2. Abre `https://TU_DOMINIO/nfc-wallet/` en **Google Chrome para Android**.
3. La primera vez toca **Activar lector NFC** y concede el permiso. En posteriores visitas el sistema intenta iniciar el escaneo automáticamente cuando el permiso ya está concedido.
4. Mantén la pantalla encendida, el teléfono desbloqueado y la pestaña visible.
5. Acerca una **etiqueta NDEF** compatible a la zona NFC del teléfono.
6. Ante un evento `reading` real, el saldo local de $100 baja $5 y se guarda un movimiento; hay un periodo de 8 segundos para evitar duplicados.
7. En **Ajustes** se puede activar el descuento **experimental** ante `readingerror`; el evento no verifica la tarjeta y puede proceder de fallas de lectura. Está **activado por defecto** para probar la idea de «cualquier tarjeta detectada»; puedes apagarlo desde Ajustes. Los cargos así generados se identifican como «no verificados» y no sirven para dinero real.

## Qué pasa con tarjetas Metro, elevador o banco

El sistema operativo puede reaccionar al acercarlas, pero Chrome **no necesariamente** entrega un evento Web NFC. En particular, **no se puede prometer detección de todas las tarjetas** por web. `readingerror` puede ocurrir con etiquetas incompatibles o por ruido/errores y no incluye una identidad verificable. Ninguna tarjeta bancaria, transporte o acceso es leída, escrita, recargada ni modificada por este sistema.

La pantalla de cobro muestra únicamente saldos y operaciones **ficticias en el mismo navegador**; el cobro no se aplica a una tarjeta ni se sincroniza entre dispositivos.

## Archivos

- `index.html`: interfaz y lógica completa, sin dependencias externas.