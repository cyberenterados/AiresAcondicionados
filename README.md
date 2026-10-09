# AirePro — servicio técnico de aire acondicionado

Landing page estática en español para presentar servicios técnicos de climatización a domicilio y recibir consultas por WhatsApp. El sitio incluye contenido de ejemplo para el negocio AirePro y puede personalizarse para un técnico o equipo de trabajo.

## Análisis del proyecto

- **Propuesta clara:** presenta diagnóstico y service, instalación y desinstalación, y limpieza y mantenimiento.
- **Recorrido comercial completo:** incluye presentación, beneficios, descripción de servicios, pasos de atención, preguntas frecuentes y llamadas a la acción.
- **Interfaz adaptable:** la hoja de estilos contempla escritorio, tablet y móvil, además de respetar la preferencia del sistema por movimiento reducido.
- **Buenas bases de accesibilidad:** idioma declarado, regiones semánticas, enlace para saltar al contenido, navegación etiquetada, estados de foco visibles y diálogo nativo para el contacto.
- **Implementación liviana:** HTML, CSS y JavaScript sin frameworks ni dependencias de instalación. Los iconos SVG y las imágenes están incorporados en el HTML, por lo que no dependen de servicios externos.

### Antes de publicar

1. Configurá `WHATSAPP_NUMBER` en `script.js` con el teléfono real en formato internacional, solo dígitos (sin `+`, espacios ni guiones). Mientras esté vacío, el formulario no tendrá un destinatario de WhatsApp válido.
2. Revisá y adaptá el nombre AirePro, los textos, los servicios, las condiciones de instalación, la zona de cobertura y los horarios. El sitio no fija una ubicación concreta.
3. La foto principal está incrustada como Base64 en `index.html`, que actualmente ocupa aproximadamente 450 KB. Para optimizar carga, conviene moverla a un archivo de imagen comprimido y referenciarlo desde el HTML.
4. Probá los enlaces y el flujo de contacto en móvil y escritorio antes de compartir el sitio.

## Estructura

- `index.html`: contenido, estructura semántica, metadatos e imágenes.
- `styles.css`: diseño visual y reglas responsive.
- `script.js`: menú móvil, diálogo de contacto, mensajes predefinidos y enlace a WhatsApp.

## Uso local

No se requiere instalar dependencias ni compilar el proyecto. Abrí `index.html` en un navegador. Para probarlo mediante un servidor local, podés ejecutar desde esta carpeta:

```bash
python -m http.server 8000
```

Luego visitá <http://localhost:8000>.

## Publicación

Se puede alojar en cualquier servicio de hosting estático. Para GitHub Pages, subí los archivos a la rama `main` y seleccioná esa rama y la carpeta raíz en **Settings → Pages** del repositorio.
