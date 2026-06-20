# KPI master CSV

Questa cartella contiene il file [`kpi_master.csv`](../kpi_master.csv), che raccoglie i principali indicatori delle tre dashboard (Economia, Immigrazione, Giustizia) in un unico CSV.

## Formato

Il file ha le seguenti colonne:

- `dashboard` — dashboard di provenienza (`economia`, `immigrazione`, `giustizia`);
- `indicator` — identificatore dell'indicatore in snake_case;
- `value` — valore numerico;
- `unit` — unità di misura (% del PIL, mld €, mln, anni, ecc.);
- `year` — anno di riferimento o periodo;
- `source` — fonte primaria (ISTAT, MEF, Banca d'Italia, Eurostat, CEPEJ, Ministeri, DAP, ISMU/Moressa, Antigone, CSM).

## Esempio

```
dashboard,indicator,value,unit,year,source
economia,debito_pil,136.4,% del PIL,2025,MEF/Banca d'Italia
giustizia,affollamento_carceri,121,% posti,2024,DAP/Antigone
```

## Come aggiornare

Quando modifichi un indicatore in una delle dashboard figlio:

1. aggiorna il valore, l'anno e la fonte nel dataset del sub-repo (`data/*.csv`);
2. aggiorna anche la riga corrispondente in `kpi_master.csv`;
3. se il dato cambia un claim narrativo, aggiorna anche `index.html` e `dashboard.html` nel sub-repo.

## Convenzioni colonne

- I valori numerici usano il punto come separatore decimale (es. `136.4`).
- Le unità sono in italiano, leggibili (% del PIL, mld €, mln, mila, anni, ecc.).
- `year` può essere un anno singolo (`2024`) o un intervallo/periodo (`media 2015-2024`, `2023-24`).
- `source` può elencare più fonti separate da `/`.

## Dataset per dashboard

Ogni sub-repo ha la propria cartella `data/` con dataset dettagliati:

- [economia-dashboard/data/](https://github.com/un-mistico/economia-dashboard/tree/main/data)
- [immigrazione-dashboard/data/](https://github.com/un-mistico/immigrazione-dashboard/tree/main/data)
- [giustizia-dashboard/data/](https://github.com/un-mistico/giustizia-dashboard/tree/main/data)