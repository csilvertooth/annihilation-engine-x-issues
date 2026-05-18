# AEX Map Editor Roadmap

This is the public roadmap for the **AEX Map Editor** (`aex_mapedit`). It
describes where the tool is going at a capability level. The Map Editor is
a standalone product with its own releases; this is a separate roadmap from
the [Unit Editor](ROADMAP.md).

> **Draft.** This roadmap is being curated and the ordering may change.
> Reactions and comments on the Map Editor tracking issue help prioritize.

The goal: grow the Map Editor from a working TNT/OTA round-trip editor into
the primary modern workstation for authoring Total Annihilation and AEX
maps — sculpt, tile, populate, validate, preview-in-engine, and package
maps, with the editor view a faithful preview of how the map plays in game.

## What works today

- Open a loose `.tnt` map, or browse maps inside
  `.hpi` / `.ufo` / `.ccx` / `.gp3` / `.gpf` archives.
- Tile view and grayscale heightmap view, swappable.
- Heights tool: raise/lower brush with configurable radius/strength.
- Features tool: place/remove features, feature catalog, add feature types.
- Tiles tool: tile palette with click-paint.
- Undo/redo for every edit.
- Save with automatic backup, Save As, and an AEX-native map format.
- Zoom/pan with cell and tile grid overlays.
- Map-centre crosshair for symmetric authoring.
- Tileset / feature library folder browsing with grouped pickers.
- Recent tiles/features.
- Live hi-res minimap preview.
- PNG / BMP minimap export with start-position overlays.
- Cross-platform (one codebase, native desktop app).

## Where it's headed

Each area is tracked by a GitHub issue. The order below is indicative.

### Engine-Accurate Map Preview
Make the editor a true WYSIWYG of the in-game view: match the engine's
projection so terrain and features sit exactly where they render in game,
with shadow/lighting parity and a dedicated "Preview In Game" view. This
is the highest priority — the editor is only trustworthy if it matches the
game.

### Archive Write & Native Map Formats
Save maps back into `.ufo` / `.hpi` / `.ccx` / `.gp3` / `.gpf` archives
(currently read-only), with a compression ladder, plus a compact
AEX-native map format. Every write path round-trip tested.

### Terrain & Heightmap Authoring
A full brush family — raise/lower, smooth, flatten, ramp, noise, falloff
curves — plus region select, height clamp, and water-level tooling.

### Tile & Texture Workbench
Stamp/pattern paint, bucket fill, autotiling and edge transitions,
per-planet palettes, minimap regeneration, and minimap image import with
TA-palette quantization.

### Feature & Resource Placement
Rectangle multi-select, copy/paste regions, scatter/density brushes, and
engine-accurate metal/energy and reclaim placement.

### Map Metadata & Game Setup
A schema-aware form editor for map metadata (start positions, planet,
wind, tidal, gravity, sun) and AEX-native map definitions, with
validation and lobby-preview parity.

### Large-Map Performance
A GPU-accelerated canvas and tiled cache so large maps (well beyond
classic TA sizes) stay responsive.

### Validation, Packaging & Publish
One-click map health reports (missing tiles/features/references, engine
readiness) and package/export profiles for legacy and AEX-native maps.

### Modern Authoring UX
Shared tool-hub experience with the Unit Editor and guided workflow
presets (e.g. "make a 2-player symmetric map", "fix a broken minimap").

## Following along

- Browse the [open issues](https://github.com/csilvertooth/annihilation-engine-x-issues/issues)
  and the Map Editor tracking issue.
- File bugs and feature requests via the
  [issue forms](https://github.com/csilvertooth/annihilation-engine-x-issues/issues/new/choose)
  — see [How to Create an Issue](docs/creating-an-issue.md).

## Further reading (Total Annihilation community)

- TA community tool listings: <https://cataclysm.tauniverse.com/index.php?p=downloads>
- Classic map-making discussion: <https://www.tauniverse.com/forum/>
