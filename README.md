# Toucan Store

Toucan Store is the master account layer for Toucan Games.

- **Toucan Games Supabase** owns authentication and the shared `account_profiles` table.
- Individual games keep their own game-specific databases.
- GSM V2 authenticates users against Toucan Games and sends the Toucan access token to its server-side bridge.
- Game-specific saves, inventory, currencies and loadouts remain in the GSM V2 project.

This keeps one account reusable across future Toucan Games without forcing every game to duplicate account credentials.

## Local preview

Open `index.html` through VS Code Live Server rather than `file://`.
