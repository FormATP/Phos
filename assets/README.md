# Sito web di PHOS E.T.S.

Sito statico (HTML, CSS e JavaScript, nessuna dipendenza e nessun build) per l'Ente del Terzo Settore **PHOS E.T.S.**

## Struttura

```
index.html          Home: chi siamo, ambiti, progetti, rete, organi, contatti
progetti.html       Schede delle candidature (H.U.B., Strade Sicure, Fuori Campo, N.E.X.T.)
trasparenza.html    Scheda dell'ente e sintesi dello statuto
css/style.css       Stili
js/main.js          Menu mobile
assets/logo.svg     Logo
.nojekyll           Disattiva Jekyll su GitHub Pages
```

## Pubblicazione su GitHub

1. Crea un nuovo repository vuoto su GitHub (ad esempio `phos-ets`).
2. Dalla cartella del sito:

```bash
git init
git add .
git commit -m "Primo commit: sito PHOS E.T.S."
git branch -M main
git remote add origin https://github.com/<TUO-UTENTE>/phos-ets.git
git push -u origin main
```

3. Su GitHub: **Settings → Pages → Build and deployment → Source: Deploy from a branch**, branch `main`, cartella `/ (root)`.
4. Dopo un minuto il sito sarà online su `https://<TUO-UTENTE>.github.io/phos-ets/`.

Per usare un dominio personalizzato, aggiungilo in **Settings → Pages → Custom domain**.

## Prova in locale

```bash
python3 -m http.server 8000
```

poi apri http://localhost:8000.

## Modifiche frequenti

- **Contatti**: cerca `phos-ets@libero.it` nei tre file `.html`.
- **Colori**: variabili all'inizio di `css/style.css`.
- **Esiti dei bandi**: quando una candidatura verrà approvata o realizzata, aggiorna il badge "Candidatura presentata" in `progetti.html` e `index.html`.
