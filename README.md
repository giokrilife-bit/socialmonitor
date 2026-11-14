# KPI social dei centri commerciali

Dashboard statica (mappa, grafici collegati, cannibalizzazione tra centri) pubblicata con GitHub Pages.

## File
- `index.html`: la dashboard. Legge `data.json`.
- `data.json`: i dati aggregati e anonimi (nessun nome di persona).
- `converti.html`: strumento per trasformare l'Excel in `data.json`. Lavora solo nel browser, non invia nulla.

## Pubblicazione (una volta sola)
1. Su GitHub crea un repository (es. `kpi-social`) e carica questi quattro file («Add file → Upload files»).
2. Vai in **Settings → Pages**, in «Build and deployment» scegli **Deploy from a branch**, ramo `main`, cartella `/ (root)`, poi Save.
3. Dopo circa un minuto la dashboard è su `https://TUONOME.github.io/kpi-social/`.
4. In **Settings → Collaborators** invita solo chi può aggiornare i dati. Attiva l'autenticazione a due fattori sul tuo account.

## Aggiornamento dei dati
1. Apri `https://TUONOME.github.io/kpi-social/converti.html`, scegli l'Excel (foglio FoglioDB) e premi «Scarica data.json».
2. Nel repository apri `data.json` → matita → oppure «Add file → Upload files», e carica il nuovo `data.json` sostituendo il vecchio. Conferma con «Commit changes».
3. Dopo circa un minuto la dashboard mostra i nuovi dati.

## Attenzione
- **Non caricare mai l'Excel originale su GitHub**: contiene i nomi delle persone e resterebbe nella cronologia anche se cancellato.
- La pagina è pubblica per chiunque abbia il link. I dati sono anonimi, ma sono comunque dati sulle provenienze: condividi il link solo con chi serve.
- Aprendo `index.html` dal computer (doppio clic) non si vedono i dati: il browser blocca la lettura di `data.json`. Usa l'indirizzo GitHub Pages.
