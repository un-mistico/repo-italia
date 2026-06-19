# Contribuire a repo_italia

Grazie per voler migliorare repo_italia. Questo progetto è aperto a correzioni, nuovi dati, nuove dashboard e miglioramenti di codice e UI.

## Come contribuire

### 1. Segnala un errore o un dato mancante

- Apri una [issue](https://github.com/un-mistico/repo-italia/issues).
- Indica il link alla dashboard o alla sezione interessata.
- Fornisci, se possibile, la **fonte primaria** e il dato corretto.
- Descrivi il problema in modo specifico: "il claim X è impreciso perché...".

### 2. Proponi una nuova dashboard

- Apri una issue con label `new-dashboard`.
- Spiega il tema, le domande a cui risponderebbe, le fonti disponibili e un esempio di 8 indicatori chiave.
- Se proponi un argomento già coperto da fonti ufficiali stabili, la probabilità che venga preso in carico è più alta.

### 3. Correggi o aggiungi dati

- I dataset sono nella cartella `data/` di ogni repository figlio.
- Ogni CSV deve contenere almeno le colonne: `valore`, `unita`, `anno`, `fonte`, `note`.
- Aggiorna anche la landing e la dashboard se il dato cambia un claim narrativo.

### 4. Migliora codice o design

- Forka il repository interessato.
- Apri una pull request chiara, descrivendo cosa cambi e perché.
- Assicurati di testare con:
  - `node --check` sugli script inline;
  - Playwright o browser reale per scroll e tab;
  - verifica che non ci siano errori nella console.

## Standard di qualità

- **Fonti:** preferiamo ISTAT, ministeri, OCSE, Eurostat, CEPEJ, Banca d'Italia, UNHCR, Frontex e istituti accreditati.
- **Caveat:** se un dato è una stima, una proiezione o ha limiti metodologici, dillo esplicitamente.
- **Neutralità:** non inserire opinioni politiche. Le "leve d'intervento" possono essere elencate come proposte tecniche dibattute, senza presa di posizione.
- **Anonimato pubblico:** non inserire nomi reali, email private o riferimenti identificabili nei contenuti pubblici.

## Processo di review

1. Ogni issue viene letto e classificato.
2. Le correzioni a errori fattuali hanno priorità alta.
3. Le nuove dashboard vengono discusse in issue prima di qualsiasi sviluppo.
4. Le PR vengono testate prima del merge.

## Domande?

Apri una issue generica o leggi il [`README.md`](./README.md).
