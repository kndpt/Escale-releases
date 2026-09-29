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

## Feedback

In Escale, **Help › Send Feedback…** opens a new issue here with your
version, build and macOS already filled in. You can also
[open one directly](https://github.com/kndpt/Escale-releases/issues/new).
Issues are public: leave out anything private (addresses of internal sites,
tokens, screenshots of your work). For something you'd rather not post,
write to hello@escalebrowser.com.

Say what you did, what you expected and what happened. If Escale crashed,
`~/Library/Application Support/Escale/crash.log` has the last trace; it
never leaves your Mac unless you attach it.

Escale began from [Search](https://github.com/driceroland/Search) by Office
Commun (MIT); both notices ship inside the app.
