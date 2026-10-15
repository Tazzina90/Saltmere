# Le Nebbie di Saltmere

Gioco investigativo testuale gotico. Si gioca dal browser e si può installare sul telefono come un'app.

## File

| File | A cosa serve |
| --- | --- |
| `index.html` | Il gioco |
| `manifest.webmanifest` | Nome, colori e icone dell'app installata |
| `sw.js` | Fa funzionare il gioco offline |
| `icons/` | Le icone |
| `.nojekyll` | Dice a GitHub Pages di pubblicare i file così come sono |

## Pubblicare su GitHub Pages

1. Crea un account gratuito su github.com, se non lo hai.
2. In alto a destra premi **+** e poi **New repository**. Chiamalo per esempio `saltmere`, lascialo **Public** e premi **Create repository**.
3. Nella pagina del repository premi **uploading an existing file**. Trascina **il contenuto** della cartella (non la cartella stessa): `index.html`, `manifest.webmanifest`, `sw.js`, `.nojekyll`, `LEGGIMI.md` e la cartella `icons`. Premi **Commit changes**.
   Se il file `.nojekyll` non si vede perché nascosto, puoi saltarlo: il gioco funziona lo stesso.
4. Vai su **Settings → Pages**. In **Build and deployment**, alla voce **Source** scegli **Deploy from a branch**, poi **Branch: main** e cartella **/ (root)**. Premi **Save**.
5. Dopo uno o due minuti, in cima a quella pagina compare il link: `https://TUONOME.github.io/saltmere/`. È il link da mandare agli amici.

## Installare sul telefono

- **iPhone (Safari):** apri il link, premi Condividi e poi **Aggiungi alla schermata Home**.
- **Android (Chrome):** apri il link, menu ⋮ e poi **Installa app** (o **Aggiungi a schermata Home**).

## Salvataggi

- Ci sono tre slot. Il gioco salva da solo dopo ogni scelta.
- I salvataggi restano sul dispositivo e nel browser in cui si gioca. Cancellando i dati del sito si perdono.
- Per spostare una partita su un altro dispositivo: **Copia codice** sullo slot, poi sull'altro dispositivo **Carica un codice** e scegli lo slot.

## Pubblicare un aggiornamento

1. Nel repository apri il file da sostituire (per esempio `index.html`), oppure usa **Add file → Upload files** e carica la nuova versione: GitHub la sostituisce.
2. Apri `sw.js` e cambia `saltmere-v1` in `saltmere-v2` (poi v3, v4…). Così telefoni e browser scaricano la versione nuova invece di tenere quella vecchia.
3. Premi **Commit changes**. Entro un paio di minuti il link mostra la versione aggiornata. I salvataggi degli amici restano validi.
