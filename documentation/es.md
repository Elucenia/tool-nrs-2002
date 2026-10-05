<!-- ELUCENIA technical documentation · nrs-2002 · es · no clinical/professional/rights approval -->

# NRS-2002

[condiciones, fuentes y permisos](https://elucenia.org/es/herramientas/nrs-2002)

## Cómo usar

Utilice la herramienta en el portal o abra index.html mediante un servidor HTTP local. Seleccione el idioma, complete los campos y calcule.

## Entradas y unidades

### Deterioro del estado nutricional

`estado`

- `0` — Ausente: estado nutricional normal
- `1` — Leve: pérdida de peso \> 5% en 3 meses o ingesta del 50% al 75% de las necesidades en la última semana
- `2` — Moderado: pérdida \> 5% en 2 meses, o IMC de 18,5 a 20,5 con estado general afectado, o ingesta del 25% al 60%
- `3` — Grave: pérdida \> 5% en 1 mes (\> 15% en 3 meses), o IMC \< 18,5 con estado general afectado, o ingesta del 0% al 25%

### Gravedad de la enfermedad (aumento de necesidades)

`gravidade`

- `0` — Ausente: necesidades nutricionales normales
- `1` — Leve: fractura de cadera, enfermedad crónica con complicación aguda (cirrosis, EPOC, hemodiálisis, diabetes, cáncer)
- `2` — Moderada: cirugía abdominal mayor, ictus, neumonía grave, neoplasia hematológica
- `3` — Grave: traumatismo craneal, trasplante de médula ósea, UCI con APACHE II \> 10

### Edad ≥ 70 años

`idade`

## Edición del método

NRS 2002/ESPEN Kondrup 2003: 2 dominios 0–3, edad≥70 +1, total 0–7

## Fórmula documentada

Puntuación = deterioro nutricional (0–3) + gravedad de enfermedad (0–3) + 1 punto si edad ≥70 años. Total 0–7.

Puntuación ≥3: riesgo nutricional.

## Límites y población

El NRS-2002 es un cribado de riesgo basado en la combinación del estado nutricional y la gravedad de la enfermedad. Su desarrollo distinguió grupos de estudios con mayor probabilidad de beneficio; un total no garantiza la respuesta individual ni prescribe la vía o la dosis de soporte nutricional. Las definiciones, la elegibilidad y la edad deben corresponder a la versión.

## Referencias

- [Kondrup J et al. Nutritional risk screening (NRS 2002): a new method based on an analysis of controlled clinical trials. Clin Nutr, 2003.](https://doi.org/10.1016/S0261-5614(02)00214-5)

- [Kondrup J et al. ESPEN guidelines for nutrition screening 2002. Clin Nutr, 2003.](https://doi.org/10.1016/S0261-5614(03)00098-0)

## Reproducir las pruebas técnicas

Ejecute node test.cjs en el directorio raíz de este repositorio para repetir los casos sintéticos registrados. Se conservan las entradas, los resultados esperados y las tolerancias originales. Las pruebas técnicas no constituyen validación clínica.

```sh
node test.cjs
```

tool.json contiene las fuentes, la edición y el alcance de la revisión. examples.json conserva las entradas y los resultados esperados de los casos sintéticos; results.json registra los resultados obtenidos.

[Ficha y referencias](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referencia](../examples.json) · [results.json](../results.json)

## Revisión y condiciones de uso

No se ha realizado una revisión clínica independiente.

Esta interfaz es una traducción de elaboración propia, no una edición oficial o certificada. No se han realizado la revisión clínica independiente, la revisión lingüística profesional ni la autorización de derechos de los instrumentos.

Resultado de la fórmula o clasificación. La interpretación, la conducta y la aplicabilidad dependen de la evaluación profesional y de la fuente seleccionada.

## Licencia y atribución

Apache-2.0 se aplica únicamente al código de ELUCENIA. Los derechos de los instrumentos, publicaciones, traducciones y datos permanecen en manos de sus respectivos titulares. Conserve LICENSE y NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
