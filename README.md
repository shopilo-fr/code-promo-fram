# Code promo FRAM, recuperation automatique depuis shopilo.fr

Module Python pour la recuperation automatique de **codes promo FRAM** depuis [shopilo.fr](https://shopilo.fr/reductions/fram.fr). Renvoie les **coupons FRAM** actifs au format JSON, pret a etre integre dans un bot Telegram, une extension de navigateur ou tout autre outil.

**Page live :** [shopilo-fr.github.io/code-promo-fram](https://shopilo-fr.github.io/code-promo-fram/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installation

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-fr/code-promo-fram
cd code-promo-fram
python fetch.py
```

## Exemple de sortie

```json
[
  {
    "store": "FRAM",
    "code": "SHOPILO15",
    "discount": "15%",
    "description": "15% de reduction sur les voyages organises",
    "expires": "2026-10-13",
    "source": "https://shopilo.fr/reductions/fram.fr"
  }
]
```

## Coupons FRAM disponibles

| Reduction | Description | Source |
|----------|-----------|-------|
| 15% | 15% de reduction sur les voyages organises | [shopilo.fr](https://shopilo.fr/reductions/fram.fr) |

Codes actifs : **[shopilo.fr/reductions/fram.fr](https://shopilo.fr/reductions/fram.fr)**

## Questions frequentes

### Comment utiliser un code promo FRAM ?
Copiez le code depuis le tableau ci-dessus ou depuis [shopilo.fr](https://shopilo.fr/reductions/fram.fr), ajoutez les produits a votre panier sur FRAM et saisissez le code au moment du paiement dans le champ prevu.

### Combien de temps durent les coupons FRAM ?
Chaque coupon a une date d'expiration indiquee dans la colonne "Expiration". Le script fetch.py renvoie uniquement les coupons actifs au moment de l'execution.

### Ou trouver les bons de reduction FRAM les plus recents ?
La page [shopilo.fr/reductions/fram.fr](https://shopilo.fr/reductions/fram.fr) est mise a jour quotidiennement avec les codes promo FRAM, bons de reduction FRAM et coupons promotionnels FRAM les plus recents.

### Le code ne fonctionne pas. Que faire ?
Verifiez la date d'expiration et les conditions (montant minimum de commande, produits eligibles). Certains codes sont valables uniquement sur l'application mobile ou pour la premiere commande.

## A propos de FRAM

FRAM est l'une des boutiques en ligne les plus populaires. Sur [shopilo.fr](https://shopilo.fr/reductions/fram.fr), retrouvez les meilleurs codes promo FRAM, coupons FRAM verifies et bons de reduction FRAM actifs, mis a jour chaque jour.

## Installation npm

```bash
npm install code-promo-fram
```

```javascript
const { fetchCoupons } = require('code-promo-fram');
fetchCoupons().then(data => console.log(data));
```

## Licence

MIT, donnees extraites de [shopilo.fr](https://shopilo.fr)
