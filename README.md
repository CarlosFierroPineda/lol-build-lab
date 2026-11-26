# LoL Build Lab

**English / Español** · An independent League of Legends build reference and item-catalog validation project.

LoL Build Lab helps players explore champion builds by role and matchup profile. The V4 prototype includes item purchase order, runes, summoner spells, situational alternatives, source links, and confidence notes. The interface starts in English and includes 🇺🇸 English / 🇲🇽 Español language buttons. Champion portraits and item catalog metadata are requested from Riot Data Dragon; statistical references link to external sources such as U.GG.

LoL Build Lab ayuda a explorar builds de campeones por posición y tipo de enfrentamiento. El prototipo V4 incluye orden de compra, runas, hechizos de invocador, alternativas situacionales, fuentes y notas sobre el nivel de confianza. La interfaz inicia en inglés e incluye botones 🇺🇸 English / 🇲🇽 Español. Los retratos y datos del catálogo se solicitan a Riot Data Dragon; las referencias estadísticas enlazan a fuentes externas como U.GG.

> This is an independent community project and is not endorsed by Riot Games. League of Legends and Riot Games are trademarks or registered trademarks of Riot Games, Inc.

## Current status / Estado actual

- Static web prototype (HTML, CSS, JavaScript) / Prototipo web estático.
- English is the default language; Spanish is available from the flag buttons / El idioma inicial es inglés; español está disponible mediante las banderas.
- Champion and item assets load from Riot Data Dragon at runtime, so an internet connection is required / Los recursos de campeones y objetos se cargan desde Riot Data Dragon y requieren internet.
- Build statistics and recommendations are reference snapshots, not live Riot API data. Verify the linked source and current patch before relying on them / Las estadísticas y recomendaciones son referencias, no datos en vivo de la API de Riot. Verifica la fuente y el parche vigente.
- The item catalog workbook in `docs/` is an early-stage working file. Seed records are marked as pending validation and are not a complete verified catalog / El Excel de objetos es un archivo de trabajo inicial; los registros semilla están pendientes de validación.
- No Riot API key is required by this prototype. Never commit API keys, passwords, tokens, or other secrets / Este prototipo no requiere API Key. Nunca publiques claves ni secretos.

## Run locally / Ejecutar localmente

1. Download or clone this repository / Descarga o clona el repositorio.
2. Open `index.html` in a modern browser while connected to the internet / Abre `index.html` en un navegador con internet.
3. If local file requests are restricted, run: `python -m http.server 8000` / Si el navegador restringe las solicitudes locales, ejecuta ese comando.
4. Visit `http://localhost:8000`.

## Publish with GitHub Pages / Publicar con GitHub Pages

1. Create a public repository, e.g. `lol-build-lab` / Crea un repositorio público.
2. Upload the contents of this folder to the repository root / Sube el contenido de esta carpeta a la raíz.
3. Open **Settings → Pages**.
4. Choose **Deploy from a branch**, branch **main**, folder **/(root)**, then save / Selecciona la rama `main` y la carpeta `/(root)`.
5. GitHub Pages will provide the public URL after deployment / GitHub Pages generará la URL pública.

## Riot API direction / Integración futura con Riot API

The current version uses Data Dragon for static game assets/data and external source links for build references; it does not yet call the League of Legends match or summoner APIs. A future Riot API integration should use appropriate key handling, server-side routing, caching, rate-limit controls, and Riot Developer Policies. Do not expose an API key in browser JavaScript or commit it to GitHub.

La versión actual usa Data Dragon para recursos estáticos y enlaces externos para las builds; todavía no consulta las APIs de partidas o invocadores. Una integración futura deberá proteger las claves, usar un servidor, caché, control de límites y cumplir las políticas de Riot.

## Project description for Riot Developer Portal

An independent web-based League of Legends build reference and item validation tool. The project helps players explore champion builds by role and matchup profile, including item purchase order, runes, summoner spells, situational alternatives, and links to statistical sources. It uses Riot Data Dragon for champion and item assets and is being developed as a non-commercial learning and prototyping project. Future versions may integrate approved Riot APIs to improve data validation and provide additional player-facing features. The project does not provide gameplay automation, unfair competitive advantages, betting, or gambling features.
