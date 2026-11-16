# Call of Duty 2: Big Red One - PC texture packs

Optional texture packs for our own engine implementation of *Call of Duty 2: Big Red One* on PC
([the game](https://github.com/SmokeDoggy044/CoD2-BRO-Native-Loader)). You need your own copy of the
game: the packs replace textures of your copy and cannot be used without it. This repository holds no code and
none of the game's data; only its releases carry the packs.

| Pack | What | Size |
|---|---|---|
| PBRify 4x textures | the levels, weapons, vehicles and characters, upscaled 4x (1,660 textures) | 605 MB |
| UI textures | menus, HUD and fonts, upscaled with models picked per texture (205 textures) | 36 MB |
| Surface maps | normal, height and surface maps for Enhanced Graphics: per-pixel lighting and shine (Vulkan renderer; needs the 4x pack) | 2.9 GB |

## Installing

Start `cod_bro_launcher` (a release with the **Texture Packs** tab: the custom engine's releases), open **Data
Files**, then the **Texture Packs** tab, and click **Install** next to each pack you want. The launcher downloads only that pack, checks every file, and can continue an interrupted download.
**Update** fetches only what changed in a new release; **Remove** deletes a pack.

Without internet on the playing PC: download the files of a release (below) by hand, put them in one folder, and
use **Install from a folder...** on the same tab.

In the game, Options > Graphics > Detail > Texture Packs turns each pack on or off (after a restart).

## Release files

Each release has the same files for all packs:

- `cod_bro_textures.index` - the list of packs and files
- `cod_bro_textures.data.001`, `.002`, ... - the packs' data
- `SHA256SUMS.txt` - checksums

The files are not usable on their own: every texture in them is encrypted with a key that only the matching
texture of the original game gives, and the game unlocks it while it loads. The format is described in
[texture-packs.md](https://github.com/SmokeDoggy044/CoD2-BRO-Decomp/blob/own_host/docs/developers/texture-packs.md).

## Credits

- PBRify 4x textures and surface maps: 4x-PBRify-UpscalerV4 and the PBRify map models (CC0).
- UI textures: 4x-AnimeSharp by Kim2091, 4x IllustrationJaNai V1 / V3 by the-database, picked per texture.
- Made with the texture pack builder of
  [CoD2-BRO-Decomp](https://github.com/SmokeDoggy044/CoD2-BRO-Decomp) (`tools/texture_pack/`) from a retail copy
  of the game.

*Call of Duty 2: Big Red One* is a trademark of Activision. This project is not affiliated with or endorsed by
Activision or Treyarch.
