# 🚀 Come deployare su GitHub Pages

Se vuoi che la tua PWA sia online gratis su GitHub Pages, ecco come fare:

## Passo 1: Crea un repository GitHub

1. Vai su [github.com](https://github.com)
2. Clicca "New repository"
3. Nomina il repo: `registro-lavoro` (o quello che vuoi)
4. Seleziona "Public"
5. Clicca "Create repository"

## Passo 2: Carica i file

### Opzione A: Con Git (terminale)

```bash
# Entra nella cartella
cd pwa-registro-lavoro

# Inizializza il repo
git init

# Aggiungi il tuo username/repo
git remote add origin https://github.com/TUO_USERNAME/registro-lavoro.git

# Carica i file
git add .
git commit -m "Prima versione PWA"
git branch -M main
git push -u origin main
```

### Opzione B: Dall'interfaccia GitHub

1. Nel tuo repo, clicca "Add file" > "Upload files"
2. Trascina tutti i file della cartella
3. Clicca "Commit changes"

## Passo 3: Attiva GitHub Pages

1. Nel repo, vai a **Settings** > **Pages**
2. Sotto "Source", seleziona **main branch**
3. Clicca **Save**
4. Aspetta 1-2 minuti

## Passo 4: Accedi alla tua app

Il sito sarà online a:  
**`https://TUO_USERNAME.github.io/registro-lavoro`**

## ✅ Fatto!

Ora la tua PWA è online. Puoi:
- 📲 Installare su mobile
- 🌐 Condividere il link
- 🔄 Aggiornare caricando nuovi file
- ✅ Funziona con HTTPS (PWA completa!)

---

**Nota:** Ogni volta che modifichi i file e fai `git push`, il sito si aggiorna automaticamente.
