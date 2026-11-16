# IQ Examen · DemosIQ

Demostración corporativa y visual de un examen en línea, optimizada para teléfonos Android y computadoras, con experiencia similar a una aplicación nativa y un flujo estilo POS.

## Estado

**Versión de demostración aprobada — 16 de noviembre de 2026.**

**Despliegue:** pendiente de conectar este repositorio a Hostinger. **No hay un sitio publicado ni una conexión de despliegue automático configurada desde aquí.**

## Inicio rápido

Abre `index.html` en un navegador moderno. También puedes subirlo a la raíz pública de un dominio; no necesita compilación, servidor de aplicaciones, base de datos ni instalación de paquetes.

## Flujo actual

1. El participante escribe su nombre.
2. Contesta **seis preguntas** básicas de matemáticas, agrupadas en **tres bloques** (sumas, restas y números).
3. Las preguntas se presentan **una por pantalla**, con tres respuestas de gran tamaño y botones **Atrás** y **Siguiente**.
4. Cada avance con **Siguiente** reproduce destellos de chispas.
5. Al completar el examen, aparecen resultados y una animación de confeti.
6. Se abre un **certificado de participación** diseñado en línea, con nombre, resultado, fecha y folio. La opción **Guardar PDF** abre el diálogo de impresión del navegador.
7. Se muestra la pantalla de **pago simulado** de $99 MXN. **No se cobra dinero.**

## Diseño aprobado

- Corporativo, limpio, intuitivo, con tarjetas grandes y navegación por pasos.
- Colores principales: azul marino, azul, blanco y acentos dorados.
- Adaptado a PC y Android, tanto vertical como horizontal.
- Sin scroll innecesario, sin formularios extensos ni menús complicados.
- Se eliminaron las tarjetas informativas inferiores “Modo” y “Acción”.
- Certificado en una sola vista, sin salir de la aplicación.
- Transiciones de chispas al avanzar y celebración más intensa al finalizar.

## Guardado y limitaciones

Usa `localStorage` para guardar **únicamente en el navegador/dispositivo** el nombre, avance, respuestas, resultado, certificado y selección de pago. Al pulsar **Reiniciar** se borra el avance de esta demostración.

No hay cuentas, sincronización entre dispositivos, panel de administración, sistema de pagos reales, validación oficial de certificados ni base de datos. El folio mostrado no se valida externamente. Todo lo anterior requiere desarrollar un backend antes de presentar el sistema como solución operativa real.

## Estructura

```text
/
├── index.html
├── README.md
└── docs/
    ├── CONTINUIDAD_IQ_EXAMEN.md
    └── DESPLIEGUE_HOSTINGER.md
```

## Publicación posterior

Ver [instrucciones de despliegue en Hostinger](docs/DESPLIEGUE_HOSTINGER.md). La rama de referencia es **main** y el archivo de entrada es **index.html**.

Proyecto de **IQneting**.