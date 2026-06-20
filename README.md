# Gestione Cassa Oratorio

App web standalone (single-file HTML) per la gestione della cassa dell'oratorio.

## Utilizzo locale

Apri direttamente il file `Gestione Cassa Oratorio (HTML standalone).html` in un browser. Non richiede installazioni né server.

## Pubblicazione su GitHub Pages

Il repository include il workflow `.github/workflows/deploy-pages.yml` che pubblica
automaticamente l'app su GitHub Pages.

Il workflow copia il file HTML standalone in `index.html` e lo pubblica. Si attiva:

- a ogni push sul branch `main`;
- manualmente da **Actions → Deploy to GitHub Pages → Run workflow**.

### Passo manuale richiesto (una sola volta)

Affinché il deploy automatico funzioni, la sorgente di GitHub Pages deve essere
impostata su **GitHub Actions**:

1. Vai su **Settings → Pages**.
2. Alla voce **Build and deployment → Source** seleziona **GitHub Actions**.

> Il workflow tenta di abilitare Pages automaticamente (`enablement: true`). Se la
> tua organizzazione/account non lo consente via API, esegui il passo manuale qui sopra.

Una volta completato il primo deploy, l'app sarà raggiungibile all'URL indicato in
**Settings → Pages** (tipicamente `https://alessandroq70.github.io/Gestione-Cassa-Oratorio/`).
