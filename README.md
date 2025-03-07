![Node build](https://github.com/eritislami/evobot/actions/workflows/node.yml/badge.svg)
![Docker build](https://github.com/eritislami/evobot/actions/workflows/docker.yml/badge.svg)
[![Commitizen friendly](https://img.shields.io/badge/commitizen-friendly-brightgreen.svg)](http://commitizen.github.io/cz-cli/)

![logo](https://repository-images.githubusercontent.com/186841818/8aa95700-7730-11e9-84be-e80f28520325)

# 🤖 DJSteven (Discord Music Bot)

> DJ Steven es un Bot de Música para Discord creado con TypeScript, discord.js y usa el Manejador de Comandos de [discordjs.guide](https://discordjs.guide)
## Requerimientos

1. Bot Token **[Guia](https://discordjs.guide/preparations/setting-up-a-bot-application.html#creating-your-bot)**  
   1.1. Habilita "Message Content Intent" en el Portal de Desarrolladores de Discord.
2. Node.js 16.11.0 o
## 🚀 Comenzando

```sh
git clone https://github.com/eritislami/evobot.git
cd evobot
npm install
```

Después de que finalice la instalación, sigue las instrucciones de configuración y luego ejecuta `npm run start` para iniciar el bot.

## ⚙️ Configuracion

Copia o Renombra `config.json.example` a `config.json` y completa los valores.:

⚠️ **Nota: Nunca compartas ni publiques tu token o claves de API.**⚠️

```json
{
  "TOKEN": "",
  "MAX_PLAYLIST_SIZE": 10,
  "PRUNING": false,
  "LOCALE": "en",
  "DEFAULT_VOLUME": 100,
  "STAY_TIME": 30
}
```

## 🐬 Configuración de Docker

Para aquellos que prefieran usar nuestro [contenedor de Docker](https://hub.docker.com/repository/docker/eritislami/evobot), pueden proporcionar los valores de `config.json` como variables de entorno.

```shell
docker run -e "TOKEN=<discord-token>" eritislami/evobot
```

## 📝 Características y Comandos

- 🎶 Reproduce música de YouTube mediante una URL.

`/play https://www.youtube.com/watch?v=GLvohMXgcBo`

- 🔎 Reproducir música de YouTube mediante una consulta de búsqueda.

`/play under the bridge red hot chili peppers`

- 🔎 Buscar y seleccionar música para reproducir.

`/search Pearl Jam`

- 📃 Reproducir listas de reproducción de YouTube mediante una URL.

`/playlist https://www.youtube.com/watch?v=YlUKcNNmywk&list=PL5RNCwK3GIO13SR_o57bGJCEmqFAwq82c`

- 🔎 Reproducir listas de reproducción de YouTube mediante una consulta de búsqueda.
`/playlist linkin park meteora`

- Now Playing (/nowplaying)
- Queue system (/queue)
- Loop / Repeat (/loop)
- Shuffle (/shuffle)
- Volume control (/volume)
- Lyrics (/lyrics)
- Pause (/pause)
- Resume (/resume)
- Skip (/skip)
- Skip to song # in queue (/skipto)
- Move a song in the queue (/move)
- Remove song # from queue (/remove)
- Show ping to Discord API (/ping)
- Show bot uptime (/uptime)
- Toggle pruning of bot messages (/pruning)
- Help (/help)
- Manejador de comandos de [discordjs.guide](https://discordjs.guide/)  
- Controles de medios mediante botones

![buttons](https://i.imgur.com/67TGY0c.png)

## 🌎 Idiomas

Los lenguajes disponibles actualmente son:

- English (en)
- Arabic (ar)
- Brazilian Portuguese (pt_br)
- Bulgarian (bg)
- Romanian (ro)
- Czech (cs)
- Dutch (nl)
- French (fr)
- German (de)
- Greek (el)
- Indonesian (id)
- Italian (it)
- Japanese (ja)
- Korean (ko)
- Minionese (mi)
- Persian (fa)
- Polish (pl)
- Russian (ru)
- Simplified Chinese (zh_cn)
- Singaporean Mandarin (zh_sg)
- Spanish (es)
- Swedish (sv)
- Traditional Chinese (zh_tw)
- Thai (th)
- Turkish (tr)
- Ukrainian (uk)
- Vietnamese (vi)
- Consulta [Contributing](#-contributing) si deseas ayudar a agregar más idiomas.  
- Para los idiomas, por favor usa el formato de dos letras [ISO 639-1](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes).

## 🤝 Contribuir

1. [Haz un fork del repositorio](https://github.com/eritislami/evobot/fork)  
2. Clona tu fork: `git clone https://github.com/tu-usuario/evobot.git`  
3. Crea tu rama de características: `git checkout -b mi-nueva-característica`  
4. Prepara los cambios: `git add .`  
5. Realiza el commit de tus cambios: `cz` O `npm run commit` no uses `git commit`  
6. Empuja los cambios a la rama: `git push origin mi-nueva-característica`  
7. Envía un pull request
