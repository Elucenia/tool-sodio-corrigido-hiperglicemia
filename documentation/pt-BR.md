<!-- ELUCENIA technical documentation · sodio-corrigido-hiperglicemia · pt-BR · no clinical/professional/rights approval -->

# Sódio corrigido na hiperglicemia

[condições, fontes e permissões](https://elucenia.org/pt-br/ferramentas/sodio-corrigido-hiperglicemia)

## Como usar

Use a ferramenta no portal ou abra index.html em um servidor HTTP local. Selecione o idioma, preencha os campos e calcule.

## Entradas e unidades

### Sódio medido

`na`

mEq/L · intervalo: 100–180

### Glicemia

`glic`

mg/dL · intervalo: 50–2000

## Edição do método

Katz 1973 fator 1,6 e Hillier 1999 fator 2,4 por 100 mg/d Lglicoseacima 100

## Fórmula documentada

Hillier: Na corrigido = Na + 2,4 × (glicose − 100) ÷ 100.

Katz: Na corrigido = Na + 1,6 × (glicose − 100) ÷ 100.

## Limites e população

Hillier 1999 estudou hiperglicemia aguda induzida em seis participantes saudáveis. A relação sódio–glicose foi não linear, sobretudo acima de 400 mg/dL; o fator médio de 2,4 não descreve com exatidão universal todas as populações e concentrações. Katz 1,6 e Hillier 2,4 são variantes distintas, apresentadas separadamente. O sódio corrigido é uma estimativa, não uma medida futura garantida nem uma prescrição da velocidade de correção.

## Referências

- [Katz MA. Hyperglycemia-induced hyponatremia: calculation of expected serum sodium depression. N Engl J Med, 1973.](https://doi.org/10.1056/NEJM197310182891607)

- [Hillier TA, Abbott RD, Barrett EJ. Hyponatremia: evaluating the correction factor for hyperglycemia. Am J Med, 1999.](https://doi.org/10.1016/S0002-9343(99)00055-8)

- [https://pubmed.ncbi.nlm.nih.gov/10225241/](https://pubmed.ncbi.nlm.nih.gov/10225241/)

## Reproduzir os testes técnicos

Execute node test.cjs na pasta raiz deste repositório para repetir os casos sintéticos registrados. As entradas, expectativas e tolerâncias originais são preservadas. Testes técnicos não constituem validação clínica.

```sh
node test.cjs
```

tool.json contém fontes, edição e escopo de revisão. examples.json conserva as entradas e expectativas sintéticas; results.json registra os resultados obtidos.

[Ficha e referências](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referência](../examples.json) · [results.json](../results.json)

## Revisão e condições de uso

Revisão clínica independente não realizada.

Esta interface é uma tradução autoral, não uma edição oficial ou certificada. Revisão clínica independente, revisão linguística profissional e autorização de direitos de instrumentos não foram realizadas.

Resultado da fórmula ou classificação. Interpretação, conduta e aplicabilidade dependem da avaliação profissional e da fonte selecionada.

## Licença e atribuição

Apache-2.0 aplica-se somente ao código da ELUCENIA. Os instrumentos, publicações, traduções e dados mantêm os direitos dos respectivos titulares. Preserve LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Resultados documentados

As informações abaixo preservam as saídas do método para exemplos sintéticos. Não constituem validação clínica independente.

### 1

Sódio corrigido normal: a hiponatremia medida se deve à glicose (translocação de água)

| Detalhes do resultado | |
| --- | --- |
| Sódio corrigido (Katz, 1,6) | 138,0 mEq/L |


### 2

Hiponatremia verdadeira mesmo após a correção

| Detalhes do resultado | |
| --- | --- |
| Sódio corrigido (Katz, 1,6) | 131,2 mEq/L |


### 3

Sódio corrigido elevado: há déficit de água livre

| Detalhes do resultado | |
| --- | --- |
| Sódio corrigido (Katz, 1,6) | 153,2 mEq/L |

