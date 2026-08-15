# Third-party notices

## Madeline 2.0 PDE (`madeline2.js`, `madeline2.wasm`)

This tool bundles a compiled copy of
[Madeline 2.0 PDE](https://github.com/piratical/Madeline_2.0_PDE), a
pedigree-layout engine, built for the browser with
[Emscripten](https://emscripten.org/) so pedigree positions are computed
by the real Madeline algorithm instead of a custom re-implementation.

- **License**: GNU General Public License, version 2 (GPLv2). Full text:
  [`LICENSE-GPL-2.0-madeline.txt`](./LICENSE-GPL-2.0-madeline.txt).
- **Original project**: https://github.com/piratical/Madeline_2.0_PDE
- **Corresponding source for this build** (patched for Emscripten;
  algorithm files themselves unmodified — see that repo's
  `README-WASM.md` for the exact diff and rationale):
  https://github.com/ryousaku/madeline2-wasm

Only Madeline's computed node positions are used; this tool's own SVG
rendering (mouse artwork, connector-line drawing) is separate,
original code and does not reuse any of Madeline's drawing/rendering
code.

## SheetJS (`xlsx.full.min.js`)

Used to parse the `.xlsx` individual-master file client-side. See
https://sheetjs.com/ for license and source.
