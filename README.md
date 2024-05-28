# Lectogram: Biblioteca Visual

` LECTOGRAM: sistema de apoyo a la ejecución de actividades de la vida diaria para personas con demencia `

### FONDEF ID23I10034
Lectogram es un proyecto diseñado para generar apoyos procedimentales para adultos con demencia en el hogar, facilitando la realización de sus tareas diarias mediante el uso de pictogramas.

Este repositorio contiene los archivos de:
- [Marca](branding.md)
- [Lugares](places.md)
- [Tareas](tasks.md)

## Estructura del repositorio
- `src/`: Contiene los archivos fuente en formato .ai (Adobe Illustrator).
  - `lectogram-branding.ai`: Logo e isotipo de marca.
  - `places.ai`: Pictogramas de lugares.
  - `tasks.ai`: Pictogramas de tareas.
- `dist/`: Contiene los archivos optimizados en formato .svg.
  - `branding/`: Pictogramas de marca optimizados (png, svg).
  - `places/`: Pictogramas de lugares optimizados.
  - `tasks/`: Pictogramas de tareas optimizados.
- `lectogram.json`: Archivo JSON con la metadata de los pictogramas.

## Uso
Para utilizar los íconos en tu proyecto, simplemente importa los archivos SVG desde la carpeta `dist` como paquete a partir de `lectogram.json`:

```json
{
  "branding": {
    "logo": "dist/branding/logo.svg"
  },
  "places": {
    "kitchen": "dist/places/kitchen.svg",
    "bedroom": "dist/places/bedroom.svg"
    // otros lugares...
  },
  "tasks": {
    "washing-dishes": "dist/tasks/washing-dishes.svg",
    "making-bed": "dist/tasks/making-bed.svg"
    // otras tareas...
  }
}
```

#### Licencia

Este proyecto está bajo la licencia de copyright de la Universidad de las Américas. Ver [licencia](LICENSE).