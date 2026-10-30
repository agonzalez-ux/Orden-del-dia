# Orden del día

Página para montar entre todo el equipo la orden del día de la reunión semanal de Bits&Atoms.

## Qué hace

- Cada persona escribe sus puntos en su tarjeta, uno por línea. Se guardan solos.
- Se cambia el día, la hora de inicio, la duración total y los minutos de bienvenida y de cierre.
- El tiempo se reparte a partes iguales entre las personas que participan. Los minutos que sobran se suman al cierre.
- El botón «Ordenar al azar» sortea el orden de las intervenciones y todos ven el mismo.
- Se puede marcar quién participa y añadir a otras personas.
- «Exportar a PDF» genera una página A4 con fondo blanco y el estilo de Bits&Atoms.

## Archivos

| Archivo | Contenido |
| --- | --- |
| `index.html` | La página completa: estilos, lógica y exportación a PDF. |

## Cómo se usa

La página está pensada para publicarse como artifact de claude.ai con estas capacidades:

- `db`: guarda la configuración (`agenda/config`) y los puntos de cada persona (`puntos/<id>`) y los comparte en directo.
- `user`: indica si la persona puede editar.
- `downloads`: permite guardar el PDF (en modo local se descarga directamente).

Para que el equipo pueda escribir, hay que compartir el artifact con permiso de colaborador. Con solo permiso de lectura, la página se ve pero no se puede editar.

Fuera de claude.ai (por ejemplo, en GitHub Pages) la página funciona en modo local: se puede editar, sortear el orden y exportar el PDF, pero los cambios solo se guardan en ese navegador y no se comparten con el resto del equipo. Para trabajar en equipo hay que usar el enlace de claude.ai.

## Dependencias

- [jsPDF 2.5.1](https://cdnjs.cloudflare.com/ajax/libs/jspdf/2.5.1/jspdf.umd.min.js) para generar el PDF.
- Fuentes Inter y JetBrains Mono desde Google Fonts.
