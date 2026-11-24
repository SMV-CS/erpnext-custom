# erpnext-custom

Eigenes ERPNext-v16-Image mit Helpdesk und CRM, gebaut von GitHub Actions.

- Apps festlegen: apps.json
- Build: Actions → "Build ERPNext image" → Run workflow (oder Änderung an apps.json pushen)
- Ergebnis: ghcr.io/smv-cs/erpnext-custom:16 (immer die neueste) und :16-<Laufnummer> (fest)
- In Coolify: Compose-Datei nutzt ghcr.io/smv-cs/erpnext-custom:16, danach Redeploy und bench --site frontend migrate im backend-Container.
