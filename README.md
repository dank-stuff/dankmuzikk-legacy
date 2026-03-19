> [!NOTE]
> This repo is the legacy code of DankMuzikk, browse the new repos at [dank-stuff/?q=dankmuzikk](https://github.com/orgs/dank-stuff/repositories?q=dankmuzikk).

<div align="center">
  <a href="https://dankmuzikk.com" target="_blank"><img src="https://dankmuzikk.com/static/android-chrome-512x512.png" width="150" /></a>

  <h1>DankMuzikk</h1>
  <p>
    <strong>Create, Share and Play Music Playlists.</strong>
  </p>
  <p>
    <a href="https://goreportcard.com/report/github.com/dank-stuff/dankmuzikk-legacy"><img alt="Go Report Card" src="https://goreportcard.com/badge/github.com/dank-stuff/dankmuzikk-legacy"/></a>
    <a href="https://github.com/dank-stuff/dankmuzikk-legacy/actions/workflows/rex-deploy.yml"><img alt="rex-deployment" src="https://github.com/dank-stuff/dankmuzikk-legacy/actions/workflows/rex-deploy.yml/badge.svg"/></a>
  </p>
</div>

## About

**DankMuzikk** is a music player designed for colloborative playlists, where a playlist's collaborators can add and vote for music in a playlist, and the other music player stuff.

## Contributing

IDK, it would be really nice of you to contribute, check the poorly written [CONTRIBUTING.md](/CONTRIBUTING.md) for more info.

## Roadmap

- [x] Search YouTube for music
- [x] Web UI
- [x] Audio player
- [x] Accounts and Profiles
- [x] Playlists
- [x] Share playlists
- [x] Vote songs in playlists
- [x] Songs queue
  - [x] Add songs to queue
  - [x] View/Edit queue
- [x] Expandable player
  - [x] Mobile
  - [x] Desktop
- [x] Share songs
- [x] Player's menu
- [ ] Update profile
- [x] Cross device control
- [ ] Offline support
- [ ] Songs' metadata fixer
- [x] Lyrics

## Technologies used

- **[Go](https://golang.org)**: Main programming language.
- **[JavaScript](https://developer.mozilla.org/en-US/docs/Web/javascript)**: Dynamic client logic.
- **[Python](https://python.org)**: Used for the YouTube download service.
- **[templ](https://templ.guide)**: The better [html/template](https://pkg.go.dev/html/template).
- **[htmx](https://htmx.org)**: The front-end library of peace.
- **[hyperscript](https://hyperscript.org)**: So htmx won't feel lonely..
- **[GORM](https://gorm.io)**: The fantastic ORM library for Golang.
- **[MariaDB](https://mariadb.org)**: Relational database.
- **[yt-dlp](https://github.com/yt-dlp/yt-dlp)**: YouTube download helper.
- **[minify](https://github.com/tdewolff/minify)**: Minify static text files.

## Run locally

1. Clone the repo.

```bash
git clone https://github.com/dank-stuff/dankmuzikk-legacy
```

2. Create the docker environment file

```bash
cp .env.example .env.docker
```

3. Create required directories

```bash
mkdir -p .db/{etc,var} .serve/{muzikkx,pix} .google-chrome-data
```

4. Run it with docker compose.

```bash
docker compose up -f docker-compose-all.yml
```

5. Visit http://localhost:20250
6. Don't ask why I chose this weird port.

## Acknowledgements

- **This project is not affiliated with YouTube or Google, or anyone to that matter in any sort of ways.**
- Colorscheme is inspired from [Dankpods](https://www.youtube.com/@DankPods)
- Loader’s CSS was made by [@thamudi](https://github.com/thamudi)
- Lyrics are provided by [LyricFind](https://www.lyricfind.com/)

---

A [DankStuff <img height="16" width="16" src="https://dankstuff.net/assets/favicon.ico" />](https://dankstuff.net) product!

Made with 🧉 by [Baraa Al-Masri](https://mbaraa.com)
