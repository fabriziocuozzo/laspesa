# GUIDA — LaSpesa su GitHub Pages
## Dal file all'app sul telefono in 10 minuti

---

## COSA HAI
- `index.html` — l'app completa
- `manifest.json` — rende l'app installabile come app vera
- `icon.png` — l'icona che appare sul telefono

---

## FASE 1 — Crea il repository su GitHub (3 min)

1. Vai su **github.com** e accedi al tuo account
2. Clicca il **+** in alto a destra → **"New repository"**
3. Compila così:
   - **Repository name:** `laspesa`
   - **Description:** Lista della spesa familiare
   - Seleziona **Public** (obbligatorio per GitHub Pages gratuito)
   - Spunta **"Add a README file"**
4. Clicca **"Create repository"**

---

## FASE 2 — Carica i file (3 min)

1. Sei nella pagina del repository appena creato
2. Clicca **"Add file"** → **"Upload files"**
3. Trascina tutti e tre i file:
   - `index.html`
   - `manifest.json`
   - `icon.png`
4. In basso scrivi nel messaggio: `Prima versione LaSpesa`
5. Clicca **"Commit changes"**

---

## FASE 3 — Attiva GitHub Pages (2 min)

1. Clicca su **"Settings"** (in alto nella pagina del repository)
2. Nel menu a sinistra cerca e clicca **"Pages"**
3. Sotto **"Branch"** seleziona **`main`** dal menu a tendina
4. Lascia la cartella su **`/ (root)`**
5. Clicca **"Save"**
6. Aspetta 1-2 minuti — poi apparirà il link:

```
https://TUOUSERNAME.github.io/laspesa/
```

> ✅ Questo è il link della tua app! Funziona su qualsiasi browser.

---

## FASE 4 — Installala sul telefono (1 min)

Manda il link via WhatsApp alla famiglia. Poi:

**Su iPhone (Safari):**
1. Apri il link in **Safari** (non Chrome!)
2. Tocca l'icona di condivisione 📤 in basso
3. Tocca **"Aggiungi alla schermata Home"**
4. Nome: `LaSpesa` → tocca **Aggiungi**

**Su Android (Chrome):**
1. Apri il link in Chrome
2. Tocca i **3 puntini** in alto a destra
3. Tocca **"Aggiungi alla schermata Home"**
4. Tocca **Aggiungi**

L'app appare con la sua icona arancione — identica a un'app vera!

---

## COME AGGIORNARE L'APP

Se vuoi modificare qualcosa (es. cambiare il PIN):

1. Vai su **github.com/TUOUSERNAME/laspesa**
2. Clicca su `index.html`
3. Clicca l'icona matita ✏️ in alto a destra
4. Modifica quello che vuoi
5. Clicca **"Commit changes"**

L'aggiornamento va online in ~1 minuto automaticamente.

---

## CAMBIARE IL PIN

Nel file `index.html`, trova questa riga:

```javascript
const PIN = "1234";
```

Cambia `1234` con il codice che vuoi. Poi salva (commit).

---

## RISOLUZIONE PROBLEMI

| Problema | Soluzione |
|----------|-----------|
| Il link non si apre | Aspetta 2-3 minuti dopo aver attivato Pages |
| L'icona non appare sul telefono | Assicurati di usare Safari (iPhone) o Chrome (Android) |
| "Errore connessione Airtable" | Controlla la connessione internet |
| La lista non si aggiorna | Tocca "Sync" in alto oppure vai in Impostazioni → Aggiorna |
| PIN errato | Controlla la riga `const PIN = "..."` nel file |

---

## RIEPILOGO

```
File da caricare:   index.html + manifest.json + icon.png
Dove:               github.com → nuovo repository "laspesa"
Attivare:           Settings → Pages → Branch: main → Save
Link finale:        https://TUOUSERNAME.github.io/laspesa/
PIN default:        1234  (cambialo in index.html)
Tempo totale:       ~10 minuti
Costo:              ZERO
```
