# CurseForge Snap

Snap packaging for [CurseForge](https://www.curseforge.com/), the mod and addon manager for games like Minecraft, World of Warcraft, The Sims 4, and more.

## Install

```bash
sudo snap install curseforge
```

Or search for **CurseForge** in the Snap Store.

## Build

Requires [Snapcraft](https://snapcraft.io/docs/snapcraft-overview).

```bash
sudo snap install snapcraft --classic
snapcraft
```

The built `.snap` file can then be installed locally:

```bash
sudo snap install --dangerous curseforge_*.snap
```

## Notes

- Confinement: strict
- Base: core24
- Architecture: amd64 only
- The upstream `.deb` is fetched directly from Overwolf at build time; the snap version tracks it automatically via `adopt-info`.
