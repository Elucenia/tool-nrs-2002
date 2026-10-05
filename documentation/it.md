<!-- ELUCENIA technical documentation · nrs-2002 · it · no clinical/professional/rights approval -->

# NRS-2002

[condizioni, fonti e autorizzazioni](https://elucenia.org/it/strumenti/nrs-2002)

## Come usare

Usi lo strumento nel portale oppure apra index.html tramite un server HTTP locale. Selezioni la lingua, compili i campi ed esegua il calcolo.

## Dati di ingresso e unità

### Compromissione dello stato nutrizionale

`estado`

- `0` — Assente: stato nutrizionale normale
- `1` — Lieve: perdita di peso \> 5% in 3 mesi o apporto dal 50 al 75% del fabbisogno nell’ultima settimana
- `2` — Moderato: perdita \> 5% in 2 mesi, oppure IMC da 18,5 a 20,5 con stato generale compromesso, oppure apporto dal 25 al 60%
- `3` — Grave: perdita \> 5% in 1 mese (\> 15% in 3 mesi), oppure IMC \< 18,5 con stato generale compromesso, oppure apporto dallo 0 al 25%

### Gravità della malattia (aumento del fabbisogno)

`gravidade`

- `0` — Assente: fabbisogno nutrizionale normale
- `1` — Lieve: frattura dell’anca, malattia cronica con complicanza acuta (cirrosi, BPCO, emodialisi, diabete, cancro)
- `2` — Moderata: chirurgia addominale maggiore, ictus, polmonite grave, neoplasia ematologica
- `3` — Grave: trauma cranico, trapianto di midollo osseo, terapia intensiva con APACHE II \> 10

### Età ≥ 70 anni

`idade`

## Edizione del metodo

NRS 2002/ESPEN Kondrup 2003: 2 domini 0–3, età≥70 +1, totale 0–7

## Formula documentata

Score = compromissione nutrizionale (0–3) + gravità della malattia (0–3) + 1 punto se età ≥70 anni. Totale 0–7.

Score ≥3: rischio nutrizionale.

## Limiti e popolazione

L’NRS-2002 è uno screening del rischio basato sulla combinazione di stato nutrizionale e gravità della malattia. Il suo sviluppo ha distinto gruppi di studi con maggiore probabilità di beneficio; un totale non garantisce una risposta individuale né prescrive la via o la dose del supporto nutrizionale. Definizioni, ammissibilità ed età devono corrispondere alla versione.

## Riferimenti

- [Kondrup J et al. Nutritional risk screening (NRS 2002): a new method based on an analysis of controlled clinical trials. Clin Nutr, 2003.](https://doi.org/10.1016/S0261-5614(02)00214-5)

- [Kondrup J et al. ESPEN guidelines for nutrition screening 2002. Clin Nutr, 2003.](https://doi.org/10.1016/S0261-5614(03)00098-0)

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
