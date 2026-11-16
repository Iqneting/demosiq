# Publicación futura: GitHub → Hostinger

**Repositorio:** https://github.com/Iqneting/demosiq
**Rama:** `main`
**Archivo público de inicio:** `index.html`

## Antes de desplegar

- Definir el dominio o subdominio de Hostinger.
- Tener el sitio creado en el hosting y acceso al panel de administración.
- Verificar la disponibilidad de la función de despliegue desde Git para el plan contratado.
- Hacer una copia de seguridad de los archivos que ya estén publicados en la carpeta del sitio, si la carpeta tiene contenido.

## Opción principal: despliegue Git desde Hostinger

1. En el panel de Hostinger, abrir la configuración Git/deployment del sitio (si está disponible en el plan).
2. Seleccionar el repositorio `https://github.com/Iqneting/demosiq.git`, la rama `main` y el directorio de destino correspondiente a la raíz pública del sitio.
3. Ejecutar el primer despliegue y comprobar que la URL del sitio muestre `index.html`.
4. Si Hostinger ofrece despliegue automático/webhook, configurar y probar esa integración **por separado**. Subir los archivos a GitHub no la activa automáticamente.

**Importante:** La ruta pública habitual es `public_html`, pero se debe confirmar la ruta real del sitio en el hosting antes de publicar para no sobrescribir otro proyecto.

## Alternativa

Si el plan o hPanel no ofrece despliegue Git, se puede descargar el repositorio y publicar `index.html` en el directorio público mediante Administrador de archivos o SFTP. Esta opción **no sincroniza automáticamente** los siguientes cambios de GitHub.

## Prueba de aceptación

- En Android: inicio, nombre, seis preguntas sin scroll innecesario ni tarjetas encimadas, transición de chispas, confeti, certificado y pantalla de pago.
- En PC: misma secuencia, diseño centrado y sin desbordes.
- Cerrar y volver a abrir para verificar que el avance permanezca en el navegador.
- Verificar que «Guardar PDF» imprima solamente el certificado.
- Confirmar que no se realizan cobros reales.

## Seguridad y alcance

Proyecto **estático, sin secretos, sin credenciales ni configuración privada en el repositorio**. Los datos de la demostración viven solo en el dispositivo. La implementación de exámenes reales con reportes por usuario, autenticación y cobros requiere backend y revisión de seguridad.

**Estado de este documento:** preparatorio. Ningún dominio ha sido conectado o desplegado desde esta entrega.