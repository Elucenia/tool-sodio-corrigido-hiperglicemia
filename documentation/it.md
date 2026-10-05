<!-- ELUCENIA technical documentation · sodio-corrigido-hiperglicemia · it · no clinical/professional/rights approval -->

# Sodio corretto nell’iperglicemia

[condizioni, fonti e autorizzazioni](https://elucenia.org/it/strumenti/sodio-corrigido-hiperglicemia)

## Come usare

Usi lo strumento nel portale oppure apra index.html tramite un server HTTP locale. Selezioni la lingua, compili i campi ed esegua il calcolo.

## Dati di ingresso e unità

### Sodio misurato

`na`

mEq/L · intervallo: 100–180

### Glicemia

`glic`

mg/dL · intervallo: 50–2000

## Edizione del metodo

Katz 1973 fattore 1,6 e Hillier 1999 fattore 2,4 per 100 mg/dL glucosio oltre 100

## Formula documentata

Hillier: Na corretto = Na + 2,4 × (glucosio − 100) ÷ 100.

Katz: Na corretto = Na + 1,6 × (glucosio − 100) ÷ 100.

## Limiti e popolazione

Hillier 1999 ha studiato l’iperglicemia acuta indotta in sei partecipanti sani. La relazione sodio–glucosio era non lineare, soprattutto oltre 400 mg/dL; il fattore medio di 2,4 non descrive con accuratezza universale tutte le popolazioni e concentrazioni. Katz 1,6 e Hillier 2,4 sono varianti distinte, presentate separatamente. Il sodio corretto è una stima, non una misurazione futura garantita né una prescrizione della velocità di correzione.

## Riferimenti

- [Katz MA. Hyperglycemia-induced hyponatremia: calculation of expected serum sodium depression. N Engl J Med, 1973.](https://doi.org/10.1056/NEJM197310182891607)

- [Hillier TA, Abbott RD, Barrett EJ. Hyponatremia: evaluating the correction factor for hyperglycemia. Am J Med, 1999.](https://doi.org/10.1016/S0002-9343(99)00055-8)

- [https://pubmed.ncbi.nlm.nih.gov/10225241/](https://pubmed.ncbi.nlm.nih.gov/10225241/)

## Riprodurre i test tecnici

Esegua node test.cjs nella cartella principale di questo repository per ripetere i casi sintetici registrati. Gli input, i risultati attesi e le tolleranze originali sono conservati. I test tecnici non costituiscono validazione clinica.

```sh
node test.cjs
```

tool.json contiene le fonti, l’edizione e l’ambito della revisione. examples.json conserva gli input e i risultati attesi dei casi sintetici; results.json registra i risultati ottenuti.

[Scheda e riferimenti](../tool.json) · [Codice JavaScript](../calculator.js) · [Casi di riferimento](../examples.json) · [results.json](../results.json)

## Revisione e condizioni d’uso

Non è stata effettuata una revisione clinica indipendente.

Questa interfaccia è una traduzione realizzata dagli autori, non un’edizione ufficiale o certificata. Non sono state eseguite la revisione clinica indipendente, la revisione linguistica professionale né la verifica delle autorizzazioni relative ai diritti sugli strumenti.

Risultato della formula o classificazione. Interpretazione, condotta e applicabilità dipendono dalla valutazione professionale e dalla fonte selezionata.

## Licenza e attribuzione

Apache-2.0 si applica solo al codice di ELUCENIA. I diritti su strumenti, pubblicazioni, traduzioni e dati restano ai rispettivi titolari. Conservi LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
