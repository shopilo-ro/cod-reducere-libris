# Cod reducere Libris — fetch automat de pe shopilo.ro

Modul Python pentru fetch automat de **coduri de reducere Libris** de pe [shopilo.ro](https://shopilo.ro/magazin/libris.ro). Returneaza **cupoane Libris** active in format JSON, gata de integrat intr-un bot Telegram, extensie de browser sau orice alt tool.

**Pagina live:** [shopilo-ro.github.io/cod-reducere-libris](https://shopilo-ro.github.io/cod-reducere-libris/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Instalare

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-ro/cod-reducere-libris
cd cod-reducere-libris
python fetch.py
```

## Output exemplu

```json
[
  {
    "store": "Libris",
    "code": "SHOPILO20",
    "discount": "20%",
    "description": "20% reducere la carti in limba engleza",
    "expires": "2026-10-02",
    "source": "https://shopilo.ro/magazin/libris.ro"
  }
]
```

## Cupoane Libris disponibile

| Reducere | Descriere | Sursa |
|----------|-----------|-------|
| 20% | 20% reducere la carti in limba engleza | [shopilo.ro](https://shopilo.ro/magazin/libris.ro) |

Codurile active: **[shopilo.ro/magazin/libris.ro](https://shopilo.ro/magazin/libris.ro)**

## Intrebari frecvente

### Cum folosesc un cod de reducere Libris?
Copiaza codul din tabelul de mai sus sau de pe [shopilo.ro](https://shopilo.ro/magazin/libris.ro), adauga produsele in cos pe Libris, si introdu codul la checkout in campul dedicat.

### Cat timp sunt valabile cupoanele Libris?
Fiecare cupon are data de expirare afisata in coloana "Expira". Scriptul fetch.py returneaza doar cupoanele active la momentul rularii.

### Unde gasesc cele mai noi voucher-uri Libris?
Pagina [shopilo.ro/magazin/libris.ro](https://shopilo.ro/magazin/libris.ro) este actualizata zilnic cu cele mai noi cod reducere Libris, voucher Libris si cupon promotional Libris.

### Codul nu functioneaza. Ce fac?
Verifica data de expirare si conditiile (valoare minima cos, produse eligibile). Unele coduri sunt valabile doar in aplicatia mobila sau pentru prima comanda.

## Despre Libris

Libris este unul dintre magazinele online populare. Gasesti pe [shopilo.ro](https://shopilo.ro/magazin/libris.ro) cele mai bune cod reducere Libris, cupoane Libris verificate si voucher Libris active, actualizate zilnic.

## Instalare npm

```bash
npm install cod-reducere-libris
```

```javascript
const { fetchCoupons } = require('cod-reducere-libris');
fetchCoupons().then(data => console.log(data));
```

## Licenta

MIT — date sursa de pe [shopilo.ro](https://shopilo.ro)
