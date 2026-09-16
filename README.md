# Práctica Calificada 2 - Desarrollo de Aplicaciones Web

Este proyecto contiene el desarrollo de la segunda práctica calificada, maquetada estrictamente con HTML5 y Tailwind CSS.

## Backlog del Proyecto (Product Backlog & Sprint Backlog)

El desarrollo se gestionó dividiendo los requerimientos en las siguientes Historias de Usuario (HU):

*   **HU01: Diseño de Bandeja de Entrada (Inbox) Responsiva.**
    *   *Tareas:* Maquetar grid de 2 columnas, aplicar breakpoints (100% en móvil, 50% en tablet, 60% en escritorio >=1400px), diseñar vistas previas de mensajes.
*   **HU02: Tarjetas de Información de Playas y Ciudades del Perú.**
    *   *Tareas:* Implementar flexbox para visualización de 10 tarjetas, calcular simetría matemática en colores de botones (hover states) e integrar grid interno de 4 imágenes por tarjeta.
*   **HU03: Landing Page E-commerce (Plantas).**
    *   *Tareas:* Construir header de navegación, cuadrícula de productos "Recién llegados" con media queries, footer completo y aplicar efectos de opacidad (+15%) en hover de imágenes.
*   **HU04: Menú Principal y Tarjetas Animadas (Index).**
    *   *Tareas:* Crear 3 tarjetas de navegación principal, programar transformación 3D simultánea (180° X y Y) simulando un card-flip, y maquetar la tabla de resumen de orden (Review Order).

## Funcionalidades por Web Page

### 1. `page01.html` (Bandeja de Entrada)
*   **Responsive Inteligente:** El grid cambia sus anchos dinámicamente según la resolución (100% en pantallas <700px, 50% entre 701px y 1399px, y 60% en pantallas >1400px).
*   **Interactividad UI:** Implementación de truncamiento automático de texto (tres puntos) en vista previa de mensajes para mantener proporciones, y sistema de favoritos (estrella) que altera el color de fondo y texto utilizando pseudo-clases de CSS sin necesidad de JavaScript.

### 2. `page02.html` (Tarjetas Flexbox)
*   **Scroll Horizontal Nativo:** Contenedores con `overflow-x-auto` y `snap` para navegar fluídamente entre las 10 tarjetas como un carrusel móvil.
*   **Composición Multi-Imagen:** Grid interno simétrico para organizar 4 imágenes por tarjeta (playas) en tamaños calculados, y estados `hover` en los botones ("Share" / "Explore" / "Full Report") usando valores alfa/opacidad matemáticamente simétricos.

### 3. `page03.html` (E-commerce Plantas)
*   **Cuadrícula Responsiva de Productos:** Grid adaptativo a 1, 2, 3 o 4 columnas dependiendo del tamaño del viewport.
*   **Efectos Visuales:** Transiciones de opacidad exactas (+15%) mediante mix-blend y escalado de transparencia al pasar el mouse por encima de los productos.

### 4. `index.html` (Página Principal)
*   **Animación 3D Avanzada:** Las tres tarjetas de enlace realizan una transformación geométrica en el espacio 3D (giro sobre eje horizontal y vertical simultáneamente) aprovechando `perspective` y `backface-visibility`.
*   **Interfaz de Orden de Compra:** Maquetación de un wizard steps estático ("Review Order", "Select Shipping", "Submit") y tabla de resumen de costos basada en grid de Tailwind.