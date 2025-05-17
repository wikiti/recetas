[![](https://github.com/wikiti/recetas/actions/workflows/deploy-site.yml/badge.svg)](https://github.com/wikiti/recetas/actions/workflows/deploy-site.yml)

# Recetas

Mi lista de recetas culinarias. De momento son solo archivos markdown, pero quizá introduzca alguna herramienta para
convertirlo en formato PDF o web.

## Prompt

Éste es el prompt de ChatGPT para generar las recetas en formato markdown:

````
Voy a pasarte texto o subir archivos de recetas culinarias. Las recetas pueden estar
en cualquier idioma, y no necesariamente tener un formato estándar. Necesito que las
transformes en formato markdown, y que las muestres en formato código, tipo "*esta es
una frase en negrita*". Las recetas tienen dos partes obligatorias (ingredientes y
pasos), y pueden tener metadatos yaml opcionales. Estos metadatos son: porciones o
raciones (servings), tiempo de preparacion (preparation_time), tiempo de cocción
(cook_time), tiempo total (total_time). Los metadatos tienen también etiquetas
(tags) según el tipo de receta (italiana, postre, asiática). Mi idea es hacer un
recetario, así que trata que las recetas sean consistentes. Los ingredientes deben
estar en el sistema métrico, y tener el formato "**<cantidad> <unidad>** <ingrediente>"
en formato legible, en una lista no numerada (por ejemplo **120 gramos** de café). Las
unidades deben estar en formato completo, no abreviadas (por ejemplo, "20 gramos" y no
"20 gr"). Los pasos deben estar numerados como una lista numerada. Cada paso debe estar
escrito con verbos imperativos ("Enciende el horno"). Puedes incluir una tercera sección
después de la sección pasos, de "consejos", que es opcional, y que solo debe incluir piezas
importantes para que la receta no salga mal. No inventes, y extrae esta información de
la receta. La suma de preparation_time y cook_time debe sumar total_time. La preparación
incluye tiempos de reposo de masas y reposo en nevera. El formato debe ser tal que así:

```
---
title: Título de la receta
servings: 2 panes
preparation_time: 15 minutos
cook_time: 1 hora 5 minutos
total_time: 1 hora 20 minutos
tags: [italiana, pan]
layout: receta
---

## Ingredientes

- **5 gramos** de harina
- **1 pizca** de sal
- ...

## Pasos

1. Mezcla todos los ingredientes en un bol.
2. Bate las claras de huevo a punto de nieve.
3. ...

## Consejos

- Intenta usar herramientas de buena calidad.
- ...
```
````
