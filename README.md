# Dashboard UTS · PETI 2026

Dashboard académico de TSI604 en un único archivo `index.html`. Contiene todos los datos, estilos personalizados y JavaScript; usa Tailwind CSS, Lucide y Chart.js vía CDN. Requiere conexión a internet para cargar esas bibliotecas. No necesita instalación, compilación, cuentas ni conexión a los Excel.

## Abrir

Abre `index.html` en un navegador moderno. Las cinco vistas también admiten enlaces directos: `#overview`, `#decision`, `#risks`, `#timeline` y `#sla`.

## Publicar en GitHub Pages

1. Crea un repositorio en GitHub y sube `index.html` a su carpeta principal.
2. En **Settings → Pages**, selecciona **Deploy from a branch**.
3. Elige la rama `main`, carpeta **/ (root)**, y guarda.
4. Cuando termine la publicación, GitHub mostrará el enlace del sitio en esa sección.

El archivo README es opcional para la publicación. No subas los Excel: el HTML ya incorpora los datos utilizados.

## Interacciones

- Cinco pestañas, enlaces internos y navegación por teclado.
- Comparación radar/barras con leyendas seleccionables y tabla ponderada.
- Matriz 5×5 con selección de riesgos, búsqueda, filtros y escenario residual propuesto.
- Gantt de 8 semanas, detalle de cada actividad, avance simulado y exportación CSV.
- Calculadora de créditos SLA con validación, escenarios rápidos y bandas resaltadas.
- Impresión de las cinco vistas, diseño adaptable y respeto por movimiento reducido.

## Datos y supuestos

El botón **Fuentes y criterios** identifica los archivos de origen, rangos y supuestos. La referencia al PETI original procede del enunciado y no de un PDF adjunto. Las especificaciones completas de requisitos y los tratamientos residuales son propuestas para validar. Todas las actividades están pendientes en las fuentes; el control de semana solo simula progreso.

El hito tiene 0 días según la solicitud, aunque el Excel de actividades registra 1 día. La integración y la instalación se solapan en S3 en el cronograma original; el dashboard señala que esto requiere una entrega parcial validada. Los 40 días corresponden al horizonte, mientras las actividades suman 55 días con trabajos en paralelo.

Los objetivos SLA son los del documento académico; no se presentan como mediciones en vivo ni como garantías oficiales de Microsoft. Las equivalencias de inactividad usan un mes de 30 días.

## Referencias técnicas

- [Tailwind Play CDN](https://tailwindcss.com/docs/installation/play-cdn). Se mantiene el CDN solicitado; Tailwind recomienda compilar los estilos para una aplicación productiva de mayor escala.
- [Chart.js: radar](https://www.chartjs.org/docs/latest/charts/radar.html).
- [Lucide para JavaScript](https://lucide.dev/guide/packages/lucide).
- [GitHub Pages: fuente de publicación](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site).
