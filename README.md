# Escale releases

Signed and notarised builds of [Escale](https://escalebrowser.com), a native
browser for developers on Mac, written in Swift on WebKit. This repository
holds releases only; Escale's source is not published here.

**Download:** [escalebrowser.com/download](https://escalebrowser.com/download)
always gives the latest disk image. macOS 14 or later.

Each release carries three files:

- `Escale.dmg` — the disk image, to install Escale;
- `Escale.zip` — what an installed Escale fetches to update itself;
- `appcast.json` — the version, build, SHA-256 of the ZIP and minimum macOS,
  read once a day by Escale through `escalebrowser.com/appcast.json`.

An update is swapped in only when its hash matches the appcast and its
signature comes from the same developer as the copy already installed.

Feedback: hello@escalebrowser.com.

Escale began from [Search](https://github.com/driceroland/Search) by Office
Commun (MIT); both notices ship inside the app.
