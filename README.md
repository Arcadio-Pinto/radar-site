# Radar di mercato: sito pubblico del progetto

Tre pagine statiche (HTML e un foglio di stile, senza JavaScript, cookie, tracciamento né risorse esterne) da pubblicare con
GitHub Pages. Servono ai portali degli sviluppatori (TikTok, Meta) come pagina del progetto, informativa sulla privacy e
condizioni d'uso. Ogni pagina è in inglese, con la versione italiana sotto (ancora `#it`).

| File | Contenuto |
|---|---|
| `index.html` | Cos'è il progetto: strumento interno, una sola persona, API ufficiali, cosa fa e cosa non fa |
| `privacy.html` | Informativa sulla privacy (GDPR) |
| `terms.html` | Condizioni d'uso essenziali |
| `style.css` | Unico foglio di stile (chiaro e scuro, leggibile da telefono) |
| `icon.png` | **Da aggiungere**: l'icona del progetto (consigliata quadrata, 512×512 px) |
| `.nojekyll` | Dice a GitHub Pages di pubblicare i file così come sono |

Questa cartella è separata dal radar: non contiene codice, dati né chiavi del radar e non va mai unita al suo repository.

## 1. Completa i segnaposto

Cerca e sostituisci in tutti e tre i file HTML (evidenziati in giallo nel browser):

- `[NOME TITOLARE]`: il tuo nome e cognome (o la ragione sociale);
- `[EMAIL DI CONTATTO]`: l'indirizzo email da mostrare ai revisori e a chi vuole esercitare i propri diritti.

Poi aggiungi `icon.png` nella cartella. Controlla il risultato aprendo `index.html` nel browser.

## 2. Crea il repository su GitHub

1. Accedi a github.com e premi **New repository** (in alto a destra, «+» → New repository).
2. Nome: per esempio `radar-site`. Visibilità: **Public** (GitHub Pages gratuito richiede un repository pubblico).
3. Non aggiungere README, .gitignore né licenza (ci sono già i file). Premi **Create repository**.

## 3. Carica i file

Da terminale, in questa cartella (sostituisci `UTENTE` con il tuo nome utente GitHub):

```bash
cd ~/radar-site
git init -b main
git add index.html privacy.html terms.html style.css icon.png .nojekyll README.md
git commit -m "Sito del progetto Radar di mercato"
git remote add origin https://github.com/UTENTE/radar-site.git
git push -u origin main
```

In alternativa, dalla pagina del repository: **Add file → Upload files**, trascina tutti i file (anche `.nojekyll`, visibile
attivando i file nascosti) e premi **Commit changes**.

## 4. Attiva GitHub Pages

1. Nel repository apri **Settings → Pages**.
2. In **Build and deployment → Source** scegli **Deploy from a branch**.
3. In **Branch** scegli `main` e la cartella `/ (root)`, poi premi **Save**.
4. Dopo uno o due minuti, in cima alla stessa pagina compare **«Your site is live at https://UTENTE.github.io/radar-site/»**.

## 5. Indirizzi da inserire nei portali

| Campo del portale | Indirizzo |
|---|---|
| Sito / URL dell'app (Website, App URL) | `https://UTENTE.github.io/radar-site/` |
| Informativa sulla privacy (Privacy Policy URL) | `https://UTENTE.github.io/radar-site/privacy.html` |
| Condizioni d'uso (Terms of Service URL) | `https://UTENTE.github.io/radar-site/terms.html` |
| Icona | carica lo stesso `icon.png` |

Apri i tre indirizzi dal telefono prima di inviarli, per controllare che rispondano.

## Nota importante

Queste sono pagine **essenziali per un uso interno** di ricerca. Se il progetto diventerà un prodotto da offrire o vendere
(con utenti, account, pagamenti o dati degli utenti), informativa sulla privacy e condizioni d'uso andranno **riscritte con un
legale**, insieme a eventuali altri adempimenti (cookie, registro dei trattamenti, nomine dei responsabili, condizioni di vendita).
