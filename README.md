# RecoveryOS — Demo

Demo statica (HTML/CSS) di **RecoveryOS**, vertical SaaS healthtech che connette ortopedici, fisioterapisti e pazienti nel recupero post-op italiano.

Questo repo serve la fase di **validation pre-MVP**: 8 pagine HTML linkate al questionario Tally per misurare interesse, willingness-to-pay e priorità feature su due lati del mercato (Fisio + Orto).

## Pagine

Punto di ingresso: [`index.html`](index.html) — landing principale con scelta Fisio / Orto.

**Lato Fisioterapista (accent terracotta)**
- [`demo-fisio-01-landing.html`](demo-fisio-01-landing.html) — landing con 6 feature, hero, value cards, network section, data moat
- [`demo-fisio-02-dashboard.html`](demo-fisio-02-dashboard.html) — dashboard pazienti con AI Priority Queue e colonna "Prossima azione"
- [`demo-fisio-03-protocolli.html`](demo-fisio-03-protocolli.html) — library protocolli di recupero

**Lato Ortopedico (accent navy)**
- [`demo-orto-01-landing.html`](demo-orto-01-landing.html) — landing con AI Resume pre-controllo come feature #1
- [`demo-orto-02-dashboard.html`](demo-orto-02-dashboard.html) — dashboard operati con AI Priority Queue e "Prossima azione"
- [`demo-orto-03-outcome-storytelling.html`](demo-orto-03-outcome-storytelling.html) — case study auto-generati con network effect block
- [`demo-orto-05-detail-giuseppina.html`](demo-orto-05-detail-giuseppina.html) — dettaglio paziente con **AI Resume block** (money shot della demo) + "Come funziona" 7 segnali

## Design system

- **Fonts**: Fraunces (display) + Manrope (body) + IBM Plex Mono (data)
- **Palette**: `--ink #0F1419`, `--bone #FBF8F2`, `--cream #F4EEDF`, `--clinical #1E3A8A` (navy primary orto), `--warmth #C2410C` (terracotta primary fisio), `--recovery #047857`, `--sun #EAB308`, `--signal #B91C1C`
- **Mobile breakpoints**: 980px e 880px (sidebar collapse, tabella compressa)
- Pulse animations su alert critici, fade-up entry animations

## Test locale

Da terminale, nella cartella del repo:

```
python -m http.server 8000
```

Poi apri `http://127.0.0.1:8000/` nel browser.

## Disclaimer

Tutti i numeri marcati con asterisco `*` sono illustrativi pre-validation, da raccogliere e validare nei primi mesi di adozione reale. I nomi pazienti e gli scenari clinici sono **dati di esempio**, non reali.

RecoveryOS supporta follow-up, comunicazione e documentazione clinica. Evidenzia pattern e anomalie nei dati raccolti, ma non fa diagnosi e non propone trattamenti. Le decisioni cliniche restano sempre al professionista.
