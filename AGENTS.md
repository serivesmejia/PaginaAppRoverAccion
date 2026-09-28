# Guía de Diseño y Construcción: Proyecto "Retro-Tech Hacker"

Este documento establece las directrices de diseño y desarrollo para replicar la estética y funcionalidad de la landing page estilo "hack@latam" (Nostalgia Digital). Todos los agentes involucrados en la creación de esta página deben seguir estrictamente estas instrucciones.

## 1. Identidad Visual y Estética ("Vibe")

*   **Concepto:** "Retro-Tech Hacker" o "Nostalgia Digital". Mezcla de minimalismo moderno con elementos retro, arte ASCII o pixel art sencillo.
*   **Atmósfera:** Nostalgia de los 90s/00s y cultura *geek*. Sensación de terminal moderno o dashboard hacker accesible.
*   **Tema Obligatorio:** *Dark Mode* estricto.
*   **Fondos:**
    *   Sólidos y oscuros.
    *   Uso ocasional de patrones sutiles: Líneas de cuadrícula (grids) arquitectónicas o tecnológicas de bajo contraste para aportar profundidad.

## 2. Paleta de Colores

El diseño debe implementarse utilizando la siguiente paleta de colores base (ideal para CSS/Tailwind):

*   **Fondo Principal:** Negro puro (`#000000`) o gris casi negro (ej. `#0A0A0A`).
*   **Texto Principal (Cuerpo):** Blanco roto o gris muy claro (ej. `#E5E5E5` o `#F3F4F6`) para maximizar la legibilidad y evitar fatiga visual.
*   **Texto de Énfasis (Títulos):** Blanco puro (`#FFFFFF`).
*   **Acentos Visuales:** Utilizar colores crudos estilo terminal (ej. verde hacker, azul eléctrico) para pequeños detalles como bordes, cursores parpadeantes o caracteres ASCII.

## 3. Tipografía (Contraste)

La jerarquía tipográfica se basa en el contraste entre fuentes con personalidad y fuentes utilitarias:

*   **Logotipo y Títulos Principales:**
    *   Estilo: Máquina de escribir, **Monospace** o **Serif retro**.
    *   Ejemplos sugeridos: *Courier New*, *IBM Plex Mono*, *Zilla Slab*.
    *   Propósito: Aportar el toque "código/hacker".
*   **Cuerpo de Texto y UI (Interfaz):**
    *   Estilo: **Sans-Serif geométrica y moderna**, de alta legibilidad.
    *   Ejemplos sugeridos: *Inter*, *Geist*, *Roboto*, *Helvetica Neue*.
    *   Detalles: Utilizar en mayúsculas espaciadas (`tracking-wider` en Tailwind) para etiquetas secundarias (ej. "ÚLTIMO LLAMADO").

## 4. Stack Tecnológico

El proyecto debe construirse utilizando las siguientes tecnologías:

*   **Framework:** **Astro** (para una landing page estática, rápida y de alto rendimiento).
*   **Estilos:** **Tailwind CSS** (utilizando utilidades como `dark:bg-black` y clases tipográficas).
*   **Lenguaje:** **TypeScript**.

## 5. Estructura y Elementos Clave (Checklist de Implementación)

La estructura de la página debe incluir obligatoriamente los siguientes elementos:

1.  **Héroe (Hero Section):**
    *   Alineación: Centrado.
    *   Contenido: Título grande (fuente monospace), subtítulo limpio (fuente sans-serif).
    *   Visual: Un elemento visual estático y evocador (ej. bloque de código formateado, un arte ASCII simple, o un logo retro pixelado).
2.  **Grids de Fondo:**
    *   Implementación: Vía CSS (`background-image: linear-gradient(...)`).
    *   Estilo: Líneas delgadas (`#333333`) sobre el fondo negro.
3.  **Contenedores y Bordes (Estilo Brutalista):**
    *   Evitar: Sombras suaves (drop-shadows) y bordes extremadamente redondeados.
    *   Aplicar: Bordes sutiles (1px sólido gris oscuro) o esquinas afiladas.
4.  **Animaciones Sutiles (Recomendado):**
    *   Implementación: Usar CSS simple (ej. cursor parpadeante al final de los textos, efectos *hover* tipo glitch ligero o cambios abruptos de color invertido).
