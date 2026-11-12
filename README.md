# DayClean site

Statisk hjemmeside for DayClean, serveret via en lille Express-server (`server.js`).

## Kør lokalt

```bash
npm install
npm start
```

Siden kører derefter på http://localhost:3000.

## Deploy på Railway

1. Push denne mappe til et GitHub-repo (eller kør `railway init` direkte i mappen hvis du bruger Railway CLI).
2. Opret et nyt projekt på [railway.app](https://railway.app) og vælg "Deploy from GitHub repo" (eller `railway up` fra CLI).
3. Railway genkender automatisk Node-projektet via `package.json` og kører `npm start`.
4. Railway sætter selv `PORT`-miljøvariablen, som `server.js` allerede lytter på.
5. Når deploy er færdig, får du en `*.up.railway.app`-URL. Et eget domæne (fx dayclean.dk) kan tilføjes under Settings → Domains.

Ingen database eller miljøvariabler er nødvendige.
