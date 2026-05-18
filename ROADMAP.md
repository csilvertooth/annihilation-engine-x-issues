# AEX Unit Editor Roadmap

This is the public roadmap for the **AEX Unit Editor**. It describes where
the tool is going at a capability level. Internal scheduling and the core
engine remain private; this document and the linked issues are the public
view.

The Map Editor is a separate standalone product with its own roadmap —
see [ROADMAP-map-editor.md](ROADMAP-map-editor.md).

The goal: grow the Unit Editor from a unit viewer/editor into the primary
modern workstation for Total Annihilation and AEX unit authoring — inspect,
edit, validate, convert, script, preview, compare, and package units
without bouncing between brittle legacy tools.

## What works today

- Layered TA data loading for loose folders and HPI-family archives
  (`.hpi`, `.ufo`, `.ccx`, `.gp3`, `.gpf`) with mod-over-base precedence.
- Unit browser with filtering, side filters, and build-pic thumbnails.
- 3DO viewport: textured rendering, team color, lighting, shadows,
  backdrops, build-pic framing, COB-driven piece transforms.
- FBI inspector with editable fields, a single Save model, a `.aexbackup`
  safety net, source restore, and change review.
- Movement-class parsing and display.
- Build Pic workflow: PCX/GAF/PNG previews, 3-frame buttons, viewport
  capture, transparent PNG export, HD PNG output.
- TA File Viewer: archive browsing, extraction, text and GAF preview.
- COB inspector/runtime + a standalone COB scripting tool (decompile,
  edit, compile, run/trace).
- Standalone Unit Compare with category filters and safe edits.

## Where it's headed

Each area below is tracked by a GitHub issue. Reactions and comments on
those issues help us prioritize.

### Field & Unit-Data Intelligence
A canonical TA/AEX field database powering hover docs, value validation,
autocomplete, safer compare-saves, and migration output. This is the
foundation the rest of the editor builds on.

### COB/BOS Scripting Workbench
Classic-Scriptor-class parity: full BOS language (preprocessor, includes,
definition files), an intelligent code editor, static analysis/linting,
and a runtime debugger with breakpoints and source mapping.

### TA File Viewer & Format Coverage
A complete, zoomable, source-aware preview and archive workbench across
every TA format — GAF, PCX, 3DO, COB/BOS, ALP, WAV/SFX, TDF, palettes —
with global search, dependency graphs, and validated repack.

### Modern Export & AEX-Native Conversion
Deliberate per-format AEX packages — 3DO→glTF model, GAF→PNG/APNG
animation, PCX/unit-pic image, COB/BOS script, FBI/weapon/moveinfo TDF
data, audio, palette, and archive→package skeleton — plus import backflow
and a dedicated Asset Converter tool (batch convert, presets, manifest
and dry-run preview, side-by-side legacy-vs-AEX render). Never silently
overwrites legacy sources.

### Validation, Packaging & Migration
One-click unit-health, missing-dependency, source-precedence, and AEX
readiness reports; a mod-package wizard; and a legacy-to-AEX migration
assistant with per-unit checklists.

### Engine-Accurate Unit Preview
A first-class orthographic "Preview Unit In Game" viewport that matches
the engine's camera, lighting, and ground contact, so creators can see
how a unit reads in game before packaging.

### Modern RTS Authoring Tooling
Layer modern code, asset, balance, validation, and package workflows over
the legacy TA data model: units edited as structured packages with full
value provenance and safe diff/merge, behavior templates for common RTS
patterns, a balance workbench with tuning charts, and one-click
package validation, test scenarios, and export profiles.

### Later
A shared online field/knowledge base and a unified tool-hub UX are on the
roadmap but not yet scheduled — they follow once the field database and
scripting workbench stabilize.

## Rough order

1. Field database foundation (unlocks lookup, validation, autocomplete,
   safer saves, migration).
2. COB/BOS editor intelligence.
3. TA File Viewer preview matrix (GAF/PCX/3DO first).
4. Validation reports.
5. Modern conversion pipeline.
6. Engine-accurate game preview.
7. Modern RTS authoring tooling.
8. Shared/online knowledge base.

## Following along

- Browse the [open issues](https://github.com/csilvertooth/annihilation-engine-x-issues/issues)
  and the per-area tracking issues.
- File bugs and feature requests via the
  [issue forms](https://github.com/csilvertooth/annihilation-engine-x-issues/issues/new/choose)
  — see [How to Create an Issue](docs/creating-an-issue.md).

## Further reading (Total Annihilation community)

- TA community tool listings: <https://cataclysm.tauniverse.com/index.php?p=downloads>
- 3DO Builder reference: <https://totalannihilation.fandom.com/wiki/3DO_Builder>
- Classic unit-making workflow discussion: <https://www.tauniverse.com/forum/showthread.php?t=30440>
- COB format/tutorial reference: <https://units.tauniverse.com/tutorials/tadesign/tadesign/cobdesc.htm>
