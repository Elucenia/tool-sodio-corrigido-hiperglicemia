<!-- ELUCENIA technical documentation · sodio-corrigido-hiperglicemia · en · no clinical/professional/rights approval -->

# Sodium corrected for hyperglycemia

[conditions, sources and permissions](https://elucenia.org/en/tools/sodio-corrigido-hiperglicemia)

## How to use

Use the tool in the portal or open index.html through a local HTTP server. Select the language, complete the fields and calculate.

## Inputs and units

### Measured sodium

`na`

mEq/L · range: 100–180

### Blood glucose

`glic`

mg/dL · range: 50–2000

## Method edition

Katz 1973 factor 1.6 and Hillier 1999 factor 2.4 per 100 mg/dL glucose above 100

## Documented formula

Hillier: corrected Na = Na + 2.4 × (glucose − 100) ÷ 100.

Katz: corrected Na = Na + 1.6 × (glucose − 100) ÷ 100.

## Limits and population

Hillier 1999 studied induced acute hyperglycemia in six healthy participants. The sodium–glucose relationship was nonlinear, especially above 400 mg/dL; the mean factor of 2.4 does not describe all populations and concentrations with universal accuracy. Katz 1.6 and Hillier 2.4 are distinct variants, presented separately. Corrected sodium is an estimate, not a guaranteed future measurement or a prescription for the correction rate.

## References

- [Katz MA. Hyperglycemia-induced hyponatremia: calculation of expected serum sodium depression. N Engl J Med, 1973.](https://doi.org/10.1056/NEJM197310182891607)

- [Hillier TA, Abbott RD, Barrett EJ. Hyponatremia: evaluating the correction factor for hyperglycemia. Am J Med, 1999.](https://doi.org/10.1016/S0002-9343(99)00055-8)

- [https://pubmed.ncbi.nlm.nih.gov/10225241/](https://pubmed.ncbi.nlm.nih.gov/10225241/)

## Reproduce the technical tests

Run node test.cjs in the root directory of this repository to repeat the recorded synthetic cases. Original inputs, expectations and tolerances are preserved. Technical tests do not constitute clinical validation.

```sh
node test.cjs
```

tool.json contains sources, edition and review scope. examples.json retains synthetic inputs and expectations; results.json records the obtained results.

[Record and references](../tool.json) · [JavaScript code](../calculator.js) · [Reference cases](../examples.json) · [results.json](../results.json)

## Review and conditions of use

Independent clinical review has not been performed.

This interface is an authorial translation, not an official or certified edition. Independent clinical review, professional language review and instrument rights clearance have not been performed.

Formula or classification result. Interpretation, care and applicability depend on professional assessment and the selected source.

## License and attribution

Apache-2.0 applies only to ELUCENIA code. Rights to instruments, publications, translations and data remain with their respective holders. Preserve LICENSE and NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Documented results

The information below preserves the method outputs for synthetic examples. It does not constitute independent clinical validation.

### 1

Corrected sodium normal: the measured hyponatremia is due to glucose (water translocation)

| Result details | |
| --- | --- |
| Corrected sodium (Katz, 1,6) | 138.0 mEq/L |


### 2

True hyponatremia even after correction

| Result details | |
| --- | --- |
| Corrected sodium (Katz, 1,6) | 131.2 mEq/L |


### 3

Corrected sodium elevated: there is free water deficit

| Result details | |
| --- | --- |
| Corrected sodium (Katz, 1,6) | 153.2 mEq/L |

