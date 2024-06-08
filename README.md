[![kibot](https://github.com/tuxuser/gh-pages-test/actions/workflows/kibot.yml/badge.svg)](https://github.com/tuxuser/gh-pages-test/actions/workflows/kibot.yml)

---

# DemoBoard

## workflows

### KiBot

[KiBot](https://github.com/INTI-CMNB/KiBot/) is used to generate all kind of documentation from a KiCAD6 project.

Whenever a file matching `pcb/*.kicad_*` changes this workflow will trigger.

The following documents are generated on every build:

```
- pcb/cad/
   - dxf/
      - AutoCAD - DXF
   - boardview - BRD
   - 3D render - STEP
- pcb/docs/
   - bom/
      - Interactive BOM - HTML
      - Octopart list - CSV
      - KiCost - XLSX (disabled)
   - schematic - PDF
- pcb/img/
   - pcb/$fab/$style/
      - PCB top - SVG
      - PCB bottom - SVG
   - render/ (disabled)
      - PCB render - PNG
   - schematic - SVG
- pcb/gerbers - ZIP
```
