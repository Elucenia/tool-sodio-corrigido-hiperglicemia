<!-- ELUCENIA technical documentation · sodio-corrigido-hiperglicemia · es · no clinical/professional/rights approval -->

# Sodio corregido en hiperglucemia

[condiciones, fuentes y permisos](https://elucenia.org/es/herramientas/sodio-corrigido-hiperglicemia)

## Cómo usar

Utilice la herramienta en el portal o abra index.html mediante un servidor HTTP local. Seleccione el idioma, complete los campos y calcule.

## Entradas y unidades

### Sodio medido

`na`

mEq/L · intervalo: 100–180

### Glucemia

`glic`

mg/dL · intervalo: 50–2000

## Edición del método

Katz 1973 factor 1,6 y Hillier 1999 factor 2,4 por 100 mg/dL glucosa sobre 100

## Fórmula documentada

Hillier: Na corregido = Na + 2,4 × (glucosa − 100) ÷ 100.

Katz: Na corregido = Na + 1,6 × (glucosa − 100) ÷ 100.

## Límites y población

Hillier 1999 estudió hiperglucemia aguda inducida en seis participantes sanos. La relación sodio–glucosa fue no lineal, sobre todo por encima de 400 mg/dL; el factor medio de 2,4 no describe con exactitud universal todas las poblaciones y concentraciones. Katz 1,6 y Hillier 2,4 son variantes distintas, presentadas por separado. El sodio corregido es una estimación, no una medición futura garantizada ni una prescripción de la velocidad de corrección.

## Referencias

- [Katz MA. Hyperglycemia-induced hyponatremia: calculation of expected serum sodium depression. N Engl J Med, 1973.](https://doi.org/10.1056/NEJM197310182891607)

- [Hillier TA, Abbott RD, Barrett EJ. Hyponatremia: evaluating the correction factor for hyperglycemia. Am J Med, 1999.](https://doi.org/10.1016/S0002-9343(99)00055-8)

- [https://pubmed.ncbi.nlm.nih.gov/10225241/](https://pubmed.ncbi.nlm.nih.gov/10225241/)

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
