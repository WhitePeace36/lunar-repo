# lunar-repo

The `[lunar]` pacman repository of [LunarOs](https://github.com/WhitePeace36/LunarOs).

The packages are not in this repository's files: they are the assets of the
release [`x86_64`](https://github.com/WhitePeace36/lunar-repo/releases/tag/x86_64),
together with the repository database (`lunar.db`, `lunar.files`) and the
signatures (`.sig`). They are built and uploaded by the scripts in LunarOs.

## Using it

Lunar systems are set up for it already: `lunar-mirrorlist` provides the
server and `lunar-keyring` the signing key. The entry in `/etc/pacman.conf`
comes before Arch's repositories:

```ini
[lunar]
Include = /etc/pacman.d/lunar-mirrorlist
```

with `/etc/pacman.d/lunar-mirrorlist`:

```ini
Server = https://github.com/WhitePeace36/lunar-repo/releases/download/x86_64
```

## Contents

Lunar's own packages (linux-lunar, lunar-settings, Elara, ananicy-cpp,
the installer, ...) and AUR packages Lunar ships. The package sources are in
[LunarOs](https://github.com/WhitePeace36/LunarOs/tree/main/packages).

Issues belong in [LunarOs](https://github.com/WhitePeace36/LunarOs/issues).
