# Railway Volume Setup

Il volume per PocketBase **non viene creato automaticamente**. Va creato manualmente una volta sola dalla dashboard Railway.

## Passaggi

1. Apri il progetto su [railway.app](https://railway.app)
2. Seleziona il servizio PocketBase
3. Vai su **Volumes** nel menu del servizio
4. Clicca **Add Volume**
5. Imposta il mount path:

```
/pb/pb_data
```

6. Salva — Railway fa il redeploy automaticamente con il volume montato

## Cosa viene persistito

Tutto ciò che PocketBase salva in `/pb/pb_data`:

- `data.db` — il database SQLite
- `storage/` — i file caricati dagli utenti
- `migrations/` — le migrazioni