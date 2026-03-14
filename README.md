# First APK

Gioco web stile Pac-Man pensato per mobile, con controlli touch e tastiera.

## Avvio locale

```bash
python3 -m http.server 8080
```

Poi apri `http://localhost:8080`.

## Build APK in GitHub Actions

Questo repository include la workflow:

- `.github/workflows/build-apk.yml`

Come usarla:

1. Vai su **Actions** nel repository GitHub.
2. Avvia la workflow **Build First APK** (anche con `workflow_dispatch`).
3. Al termine, scarica l'artifact `first-apk-debug`.
4. Dentro trovi `app-debug.apk` installabile su Android.

## Note tecniche

- Packaging Android con Capacitor.
- Config app in `capacitor.config.json`.
- Asset web copiati in `dist/` tramite `npm run build:web`.
