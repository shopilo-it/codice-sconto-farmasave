# Codice sconto FarmaSave, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto FarmaSave** da [shopilo.it](https://shopilo.it/negozi/farmasave.it). Restituisce **coupon FarmaSave** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-farmasave](https://shopilo-it.github.io/codice-sconto-farmasave/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-farmasave
cd codice-sconto-farmasave
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "FarmaSave",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% di sconto su parafarmaci",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/farmasave.it"
  }
]
```

## Coupon FarmaSave disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 10% | 10% di sconto su parafarmaci | [shopilo.it](https://shopilo.it/negozi/farmasave.it) |

Codici attivi: **[shopilo.it/negozi/farmasave.it](https://shopilo.it/negozi/farmasave.it)**

## Domande frequenti

### Come utilizzo un codice sconto FarmaSave?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/farmasave.it), aggiungi i prodotti al carrello su FarmaSave e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon FarmaSave?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher FarmaSave piu recenti?
La pagina [shopilo.it/negozi/farmasave.it](https://shopilo.it/negozi/farmasave.it) viene aggiornata quotidianamente con i codici sconto FarmaSave, voucher FarmaSave e coupon promozionali FarmaSave piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su FarmaSave

FarmaSave e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/farmasave.it) trovi i migliori codici sconto FarmaSave, coupon FarmaSave verificati e voucher FarmaSave attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-farmasave
```

```javascript
const { fetchCoupons } = require('codice-sconto-farmasave');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
