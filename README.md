# 📱 Registro Lavoro - PWA

Questa è una **Progressive Web App** (PWA) per gestire il tuo registro di lavoro, trasferte, assenze e busta paga.

## 🎯 Caratteristiche

✅ **Installabile** - Installala come app sul tuo telefono  
✅ **Offline** - Funziona senza connessione internet  
✅ **Veloce** - Carica istantaneamente dalla cache  
✅ **Responsive** - Perfetto su mobile, tablet e desktop  
✅ **Sicura** - I tuoi dati rimangono nel tuo dispositivo  

---

## 📂 Struttura della cartella

```
pwa-registro-lavoro/
├── index.html              ← La tua app (HTML+CSS+JS)
├── manifest.json           ← Configurazione PWA
├── service-worker.js       ← Motore offline + cache
└── README.md               ← Questo file
```

---

## 🚀 Come usarla

### **Opzione 1: Localmente sul tuo PC**

1. Scarica tutta la cartella `pwa-registro-lavoro`
2. Apri `index.html` con un browser (Chrome, Firefox, Edge)
3. L'app funziona subito!

### **Opzione 2: Online (consigliato per PWA completa)**

Per attivare tutte le funzioni PWA (installazione, offline):

1. **Carica i file sul tuo sito web** (es. tramite FTP, GitHub Pages)
2. Assicurati di usare **HTTPS** (richiesto dalle PWA)
3. Apri il sito dal browser mobile
4. Clicca "Installa" quando ti appare il prompt
5. L'app sarà nella home screen come app vera

### **Opzione 3: Con un server locale (dev)**

Se vuoi testare localmente con HTTPS:

```bash
# Con Python 3
python -m http.server 8000

# Con Node.js
npx http-server -p 8000
```

Poi apri: `http://localhost:8000`

---

## 📲 Come installare su mobile

### **Android (Chrome/Edge)**
1. Apri il sito da mobile
2. Vedrai un popup "Installa" o clicca i tre puntini > "Installa app"
3. Conferma
4. L'app appare in home screen

### **iPhone/iPad (Safari)**
1. Apri il sito da Safari
2. Clicca il pulsante Condividi
3. Seleziona "Aggiungi alla schermata Home"
4. Scegli il nome e conferma

---

## ⚙️ Come personalizzare

### **Cambiare il nome/colore dell'app**

Modifica `manifest.json`:
```json
{
  "name": "Il tuo nuovo nome",
  "theme_color": "#123456",  ← Colore barra in alto
  "background_color": "#ffffff"  ← Colore sfondo
}
```

### **Aggiungere un'icona personalizzata**

Sostituisci gli SVG nei `"src"` di manifest.json con link a file PNG:
```json
"src": "icons/icon-192x192.png",
"sizes": "192x192",
"type": "image/png"
```

---

## 🔄 Aggiornamenti

La PWA si aggiorna automaticamente quando metti nuovi file sul server.
Se vuoi forzare un aggiornamento:

1. Cancella i dati dell'app (Impostazioni > App > Registro Lavoro > Memoria)
2. Riapri l'app

---

## 💾 I tuoi dati

Tutti i dati (registri, trasferte, assenze) sono salvati **localmente nel tuo dispositivo** usando `localStorage`.
Nessun dato viene inviato a server esterni.

**Backup**: Puoi esportare/importare i dati direttamente dall'app.

---

## 🛠️ Cosa contiene questa PWA

- **index.html** - L'interfaccia completa della tua app
- **manifest.json** - Dice al sistema che è un'app installabile
- **service-worker.js** - Gestisce la cache e il funzionamento offline

---

## 📊 Browser supportati

| Browser | Mobile | Desktop |
|---------|--------|---------|
| Chrome | ✅ | ✅ |
| Firefox | ✅ | ✅ |
| Edge | ✅ | ✅ |
| Safari (iOS 15+) | ✅ | ✅ |
| Samsung Internet | ✅ | - |

---

## ❓ Domande frequenti

**D: Funziona senza internet?**  
R: Sì! Una volta caricata, funziona offline. I nuovi dati vengono salvati localmente.

**D: Dove sono salvati i miei dati?**  
R: Nel tuo dispositivo, in una memoria sicura (localStorage). Nessun cloud.

**D: Come faccio a sincronizzare su più dispositivi?**  
R: Puoi esportare i dati come JSON e importarli su un altro dispositivo.

**D: Posso metterla su Google Play Store?**  
R: Sì, ma richiederebbe un wrapper Android (Cordova/Capacitor). Non è necessario per una PWA.

---

## 📝 Licenza

Usa questa app come preferisci. È tua!

---

**Creata il:** maggio 2026  
**Tipo:** Progressive Web App  
**Tecnologie:** HTML5 + CSS3 + JavaScript + Service Workers
