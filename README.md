## Usage

Clone this repo into your `void-packages/srcpkgs` folder with the following commands:

```bash
cd void-packages/srcpkgs
git clone https://git.deadzone.lol/Wizzard/librewolf-void.git librewolf
```

Then build with:

```bash
cd ../../
./xbps-src pkg librewolf
```

For `aarch64` cross package build:

```bash
./xbps-src -a aarch64 pkg librewolf
```

## Auto Updates

The `.gitea/workflows/update.yml` workflow tracks LibreWolf `bsys6` releases and updates:

- `version`
- `_rev`
- `x86_64` checksum
- `aarch64` checksum
