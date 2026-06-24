# 🇮🇹 repo_italia

**Dati, fatti e numeri per capire l'Italia.**

repo_italia è un hub open source di data journalism che raccoglie dashboard pubbliche, dati scaricabili e metodologia trasparente su economia, immigrazione e giustizia in Italia.

🌐 **Sito pubblico:** [https://un-mistico.github.io/repo-italia/](https://un-mistico.github.io/repo-italia/)

---

## Cosa trovi qui

| Dashboard | Tema | URL |
|---|---|---|
| 💰 Economia | Ricchezza, debito, spesa pubblica, Superbonus, tasse, disuguaglianze, lavoro, produttività | [economia-dashboard](https://un-mistico.github.io/economia-dashboard/) |
| 🚢 Immigrazione | Presenza, confronto UE, rotte, origini, rimpatri, criminalità, conti pubblici | [immigrazione-dashboard](https://un-mistico.github.io/immigrazione-dashboard/) |
| ⚖️ Giustizia | Denunce, reati irrisolti, forze dell'ordine, processi, carceri, magistrati, costi | [giustizia-dashboard](https://un-mistico.github.io/giustizia-dashboard/) |

Ogni dashboard ha:

- una **landing scrolly-telling** per raccontare gli indicatori chiave (8 per economia e immigrazione, 7 per giustizia);
- una **dashboard completa** con grafici, tabelle e confronti;
- **dataset CSV** scaricabili con fonti e metodologia;
- **glossario e caveat** per leggere i numeri senza farsi ingannare.

---

## Filosofia

- **Zero opinioni, dati chiari.** Non facciamo politica. Mostriamo numeri, fonti e limiti.
- **Open source.** Codice, dati e metodologia sono pubblici sotto licenza CC BY 4.0.
- **Trasparenza metodologica.** Ogni indicatore indica anno di riferimento, fonte primaria e caveat interpretativi.
- **Community driven.** Chiunque può segnalare errori, proporre nuovi dati o suggerire nuove dashboard.

---

## Repository collegati

- [un-mistico/economia-dashboard](https://github.com/un-mistico/economia-dashboard)
- [un-mistico/immigrazione-dashboard](https://github.com/un-mistico/immigrazione-dashboard)
- [un-mistico/giustizia-dashboard](https://github.com/un-mistico/giustizia-dashboard)

---

## KPI master

Il file [`kpi_master.csv`](./kpi_master.csv) contiene i principali indicatori delle tre dashboard in un unico CSV, utile per analisti, giornalisti e ricercatori.

Il formato del file è documentato in [`data/README.md`](./data/README.md).

---

## Licenza

I **dati** provengono da fonti pubbliche (ISTAT, ministeri, OCSE, Eurostat, CEPEJ, UNHCR, Frontex e altri) e sono riportati in buona fede.

I **testi, grafici e codice** di repo_italia sono rilasciati sotto [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/deed.it): puoi riusarli citando la fonte.

---

## Contribuire

Vedi [`CONTRIBUTING.md`](./CONTRIBUTING.md).

Per segnalare un errore o proporre un dato, apri una [issue](https://github.com/un-mistico/repo-italia/issues).

---

## Aggiornamenti

**Giugno 2026**
- Nuova dashboard Giustizia: 8 indicatori su denunce, processi, carceri, magistrati, costi ed efficienza del sistema giudiziario
- Fix UI/UX su tutte le landing: barre proporzionali con scala zero-based, allineamento etichette, scroll-snap ripristinato
- Aggiunti dati verificati: polizia (Eurostat), sovraffollamento carcerario (Antigone), custodia cautelare, recidiva, PM (CEPEJ), digitalizzazione, autori ignoti (ISTAT)
- Landing Immigrazione: toggle macro-aree di default, chart ratio denunce/presenza con 6 paesi, dati rotte e rimpatri allineati con fonti
- Landing Economia: scale barre corrette, colori consistenti (Italia accent, altri neutral)

**Maggio 2026**
- Rilancio hub repo_italia con 3 dashboard: Economia, Immigrazione, Giustizia
- KPI master CSV con indicatori chiave delle tre aree

---

## Disclaimer

Non tutti i numeri pubblici sono ugualmente robusti. Prima di citare i dati in pubblico, verifica sempre le **fonti primarie** indicate in ogni dashboard.
