# Ciclos de vida, la biología día a día

Colección de animaciones 3D interactivas que muestran el ciclo de vida de distintas especies, etapa por etapa, con tamaños a escala y duraciones citadas de fuentes científicas.

Hechas con [three.js](https://threejs.org) r128. No necesitan instalación: se abre `index.html` en el navegador o se publican con GitHub Pages.

## Especies disponibles

| Especie | Carpeta | Fuentes |
|---|---|---|
| Mariposa monarca (*Danaus plexippus*) | [`monarca/`](monarca/index.html) | Monarch Joint Venture y Monarch Watch (Universidad de Kansas) |

## Controles de la monarca

- Reproducir o pausar con el botón o la barra espaciadora.
- Arrastrar la línea de tiempo para ir a cualquier día.
- Flechas izquierda y derecha para moverse de 6 en 6 horas.
- Cámara guiada encendida o apagada para girar y hacer zoom libremente.

## Cómo sumar otra especie

1. Crear una carpeta nueva con el nombre de la especie, por ejemplo `rana/`, con su propio `index.html`.
2. Agregar en esa página un enlace de regreso a `../`.
3. Sumar una tarjeta en el `index.html` de la raíz y una miniatura en `assets/`.
4. Citar las fuentes de cada dato en la propia página de la especie.

**Regla de contenido:** toda duración, tamaño o comportamiento tiene fuente. Si no la hay, no se pone.

## Estado

Hoy cada especie es una página independiente y la monarca lleva su escena dentro de su propio archivo. El siguiente paso lógico es extraer el motor (cámara, línea de tiempo, controles) a un archivo común y dejar cada especie como un archivo de datos con sus etapas. Con eso, sumar una especie sería escribir datos y modelar su cuerpo, no copiar toda la página.
