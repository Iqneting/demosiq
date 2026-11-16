# Continuidad maestra · IQ Examen

**Fecha:** 16 de noviembre de 2026
**Repositorio:** https://github.com/Iqneting/demosiq
**Rama principal:** `main`
**Estado:** maqueta HTML funcional aprobada para presentar a clientes, pendiente de despliegue en Hostinger.

## Alcance aprobado

- Experiencia tipo aplicación Android nativa, igualmente elegante en PC.
- Diseño corporativo, simple, principalmente gráfico y con el mínimo texto.
- Navegación paso a paso: una pregunta a la vez, tres respuestas visuales, botón Siguiente.
- Tres bloques de matemáticas muy básicas, con seis preguntas en total.
- Guardado local automático en el navegador.
- Destello de magia/chispas cada vez que se avanza con Siguiente.
- Confeti de impacto cuando se termina el examen.
- Resultado y certificado personalizado con visualización integrada.
- Botón Guardar PDF mediante impresión del navegador.
- Pago simulado posterior al certificado.

## Correcciones aprobadas

1. Eliminados los recuadros inferiores “Modo demostración” y “Acción”.
2. Corregida la distribución de tarjetas en Android para evitar elementos encimados.
3. Las transiciones agregan chispas al avanzar, sin interrumpir la respuesta.
4. Certificado vuelto a presentar en línea, en una sola pieza y con más diseño.
5. Mantener apariencia corporativa: no infantilizar, no sobrecargar con textos.

## Reglas permanentes de UX

- Priorizar tarjetas y botones grandes en vez de formularios nativos tediosos.
- Evitar scroll vertical u horizontal innecesario y contenido superpuesto.
- El cliente debe entender y recorrer la demo rápidamente.
- No agregar textos de demostración redundantes en la interfaz principal.
- No cambiar el flujo aprobado sin autorización expresa.
- Respetar los colores y el estilo visual de la versión aprobada.

## Límites técnicos actuales

Todo está contenido en `index.html` (HTML + CSS + JavaScript). Usa `localStorage`; **no existe base de datos, backend, pagos reales ni validación de certificados**. En esta etapa no se debe presentar como sistema de exámenes multiusuario en producción.

## Siguiente paso solicitado

Preparar enlace del repositorio GitHub **demosiq** con Hostinger en un paso posterior, utilizando rama `main`. **Este paso no forma parte de la publicación actual** y no se ha configurado ningún despliegue desde este documento.