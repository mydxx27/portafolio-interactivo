# Portafolio Interactivo — Estudio de Dirección de Arte & Branding

Landing page responsiva desarrollada para presentar los servicios y proyectos de un estudio creativo de dirección de arte, identidad visual, packaging y experiencia web, integrando Bootstrap 5 y efectos avanzados en CSS3 puro.

## 1. Estructura Responsiva con Bootstrap 5
- **Navbar (`bg-dark`):** Barra superior con identidad del proyecto (`Portafolio Interactivo`), enlaces de navegación (`Inicio`, `Proyectos`, `Contacto`) y colapso automático en menú tipo hamburguesa para dispositivos móviles.
- **Sistema de Grid:** Maquetación adaptable mediante `container`, `row`, `col-sm-12`, `col-md-6`, `col-lg-4`, `col-lg-5` y `col-lg-7` sin desbordamiento horizontal.
- **Formulario de Contacto y Botones:** Ubicado en la sección inferior empleando `mb-3`, `form-label` y `form-control` para los campos Nombre, Email y Mensaje, junto con los botones `Enviar` (`btn btn-primary`) y `Limpiar` (`btn btn-secondary`) distribuidos con `d-grid gap-2`.

## 2. Transformaciones 2D, 3D y Transiciones CSS
- **Transformaciones 2D al pasar el cursor (`:hover`):** Aplicadas en las tarjetas principales de la sección de Proyectos con `transition` de `0.4s ease` para suavizar el movimiento:
  - **Caja 01 (`.caja-rotacion` - Velvet Botanicals):** Rotación suave mediante `transform: rotate(-3deg)`.
  - **Caja 02 (`.caja-escalado` - Aurelia Skincare):** Escalado mediante `transform: scale(1.05)`.
  - **Caja 03 (`.caja-traslacion` - Nomad Studio):** Traslación combinada con sesgado mediante `transform: translateY(-10px) skewX(-2.5deg)`.
- **Transformación 3D:** Aplicada en el retrato principal de portada mediante el contenedor padre `.contenedor-3d` con `perspective: 1000px` y el contenedor hijo `.tarjeta-3d` con `transform-style: preserve-3d`, ejecutando `transform: rotateX(11deg) rotateY(-14deg)` al pasar el cursor y desplazando la etiqueta frontal en profundidad con `translateZ(42px)`.

## 3. Animaciones CSS Avanzadas (`@keyframes`)
- **Animación de Carga / Loader (`@keyframes giroContinuo`):** Spinner circular infinito ubicado al inicio de la página (`.loader-spinner`) y sello editorial giratorio (`.sello-giratorio`), configurados con `animation-duration`, `animation-timing-function: linear`, `animation-iteration-count: infinite` y `animation-direction: normal`.
- **Animación Personalizada de Pulso (`@keyframes pulsoEditorial`):** Aplicada a la insignia `.etiqueta-animada`, alternando escala y color continuamente mediante `animation-duration: 2.4s`, `animation-timing-function: ease-in-out`, `animation-iteration-count: infinite` y `animation-direction: alternate`.
- **Animación de Entrada (`@keyframes aparicionEditorial`):** Desplazamiento vertical suave del encabezado principal `.titulo-portafolio` al cargar la página (`animation-duration: 1.1s`, `animation-timing-function: ease-out`, `animation-iteration-count: 1`).