# Codice sconto Sarenza, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto Sarenza** da [shopilo.it](https://shopilo.it/negozi/sarenza.it). Restituisce **coupon Sarenza** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-sarenza](https://shopilo-it.github.io/codice-sconto-sarenza/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-sarenza
cd codice-sconto-sarenza
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "Sarenza",
    "code": "SHOPILO15",
    "discount": "15%",
    "description": "15% di sconto su calzature firmate",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/sarenza.it"
  }
]
```

## Coupon Sarenza disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 15% | 15% di sconto su calzature firmate | [shopilo.it](https://shopilo.it/negozi/sarenza.it) |

Codici attivi: **[shopilo.it/negozi/sarenza.it](https://shopilo.it/negozi/sarenza.it)**

## Domande frequenti

### Come utilizzo un codice sconto Sarenza?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/sarenza.it), aggiungi i prodotti al carrello su Sarenza e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon Sarenza?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher Sarenza piu recenti?
La pagina [shopilo.it/negozi/sarenza.it](https://shopilo.it/negozi/sarenza.it) viene aggiornata quotidianamente con i codici sconto Sarenza, voucher Sarenza e coupon promozionali Sarenza piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su Sarenza

Sarenza e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/sarenza.it) trovi i migliori codici sconto Sarenza, coupon Sarenza verificati e voucher Sarenza attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-sarenza
```

```javascript
const { fetchCoupons } = require('codice-sconto-sarenza');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
