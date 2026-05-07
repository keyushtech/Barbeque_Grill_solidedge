# Barbeque Grill — CAD Assembly

A flat-pack, charcoal-style barbeque grill designed in **Siemens Solid Edge** as a group project under the **MEP102 (Digital Fabrication)** course at IIT Bhilai. The assembly consists of 8 unique parts that slot together without fasteners, forming a fully functional tabletop grill with a cooking grate, charcoal mesh, ash tray, side stands, and a handle.

Exploded views are included as rendered PNG images for reference and presentation.

---

## Project Structure

```
Barbeque Grill/
├── MEP_project.asm          # Top-level Solid Edge assembly file
├── MEP_project.dft          # 2D draft/engineering drawing
├── MEP_project.cfg          # Assembly configuration
├── mep1.par                 # Cooking grate (top grill grid)
├── mep2.par                 # Charcoal mesh / fire grate
├── mep3.par                 # Firebox body (vented)
├── mep4.par                 # Side stand panel (×2 in assembly)
├── mep5.par                 # Ash / drip tray (orange)
├── mep6.par                 # Cross support legs (×2 in assembly)
├── mep7.par                 # Handle bracket
├── mep8.par                 # Handle rail
├── Credits.txt              # Team member contributions
├── Exploded_view1.png       # Exploded view — isometric angle 1
├── Exploded_view2.png       # Exploded view — isometric angle 2
└── Exploded_view3.png       # Exploded view — isometric angle 3
```

---

## Components

| Part | File | Description | Designer |
|------|------|-------------|----------|
| **Cooking Grate** | `mep1.par` | Top-level ribbed grill grid where food is placed; features a dense parallel-bar pattern | Keyush Sai |
| **Charcoal Mesh** | `mep2.par` | Fine mesh grate that sits below the cooking grate; holds charcoal while allowing airflow | Keyush Sai |
| **Firebox Body** | `mep3.par` | Central vented rectangular body that encloses the charcoal bed; slots into the side stands | Malank |
| **Side Stand Panel** | `mep4.par` | Triangular bracket-style side panel with notched slots; two instances used in the assembly | Abhishek Ujval |
| **Ash Tray** | `mep5.par` | Rectangular tray that slides under the firebox to collect ash and embers | Malank |
| **Cross Support Legs** | `mep6.par` | Diagonal cross-leg supports that slot into the side panels to form the base frame | Saumitra (completed by Keyush Sai) |
| **Handle Bracket** | `mep7.par` | Side-mounted bracket that connects the handle rail to the firebox body | Srikar & Keyush Sai |
| **Handle Rail** | `mep8.par` | Top horizontal handle rail with grip; most geometrically complex part in the assembly | Vivek |

> Assembly, exploded view configuration, and final integration: **Keyush Sai** (support: Malank)

---

## Assembly Overview

The grill is a layered, slot-together assembly built from the base up:

```
[ Handle Rail      (mep8)   ]
[ Handle Bracket   (mep7)   ]
────────────────────────────────────
[ Cooking Grate    (mep1)   ]  ← Food sits here
[ Charcoal Mesh    (mep2)   ]  ← Charcoal sits here
[ Firebox Body     (mep3)   ]  ← Encloses the fire
[ Ash Tray         (mep5)   ]  ← Collects ash below
────────────────────────────────────
[ Side Stand Panels (mep4 ×2) ] + [ Cross Support Legs (mep6 ×2) ]
                                   ← Base frame
```

1. The two **Side Stand Panels** (mep4) and **Cross Support Legs** (mep6) interlock to form a rigid A-frame base.
2. The **Firebox Body** (mep3) rests on the stands, with vent slots on the sides for airflow.
3. The **Ash Tray** (mep5) slides underneath the firebox to catch falling ash.
4. The **Charcoal Mesh** (mep2) sits inside the firebox to support the charcoal bed.
5. The **Cooking Grate** (mep1) rests on top, providing the grilling surface.
6. The **Handle Bracket** (mep7) and **Handle Rail** (mep8) attach on the sides for lifting and carrying.

---

## Exploded Views

Three rendered exploded views are included in the project folder:

| File | Angle |
|------|-------|
| `Exploded_view1.png` | Isometric — front-left perspective |
| `Exploded_view2.png` | Isometric — front-right perspective |
| `Exploded_view3.png` | Isometric — elevated top-down perspective |

These can be used directly in reports, presentations, or documentation without needing to open the CAD files.

---

## File Formats

| Extension | Format | Purpose |
|-----------|--------|---------|
| `.asm` | Solid Edge Assembly | Defines all part placements, constraints, and the assembly tree |
| `.dft` | Solid Edge Draft | 2D engineering drawing with orthographic views and dimensions |
| `.cfg` | Configuration file | Assembly display and environment settings |
| `.par` | Solid Edge Part | Parametric 3D solid model for each individual component |

---

## Software Requirements

- **Siemens Solid Edge** (any recent version) — for full editing and assembly management
- **Solid Edge Viewer** — free read-only viewer (available from Siemens)
- For cross-platform use, export to **STEP (`.stp`)** or **STL** from Solid Edge for use in Fusion 360, SolidWorks, FreeCAD, or 3D printing slicers

---

## Opening the Assembly

1. Extract the ZIP — keep all `.par` files in the **same folder** as `MEP_project.asm`.
2. Open Solid Edge and load `MEP_project.asm`.
3. Solid Edge will resolve all part references automatically from the same directory.
4. To view the engineering drawing, open `MEP_project.dft`.

> **Note:** The original files were authored on macOS. Opening on Windows for the first time may trigger a path re-link dialog — point it to the folder containing the `.par` files.

---

## Team Credits

| Contributor | Contributions |
|-------------|---------------|
| **Keyush Sai** | mep1, mep2, mep6 (completion), mep7 (co-design), full assembly & exploded views |
| **Malank** | mep3, mep5, assembly support |
| **Abhishek Ujval** | mep4 |
| **Saumitra** | mep6 (initial, incomplete) |
| **Srikar** | mep7 (co-design) |
| **Vivek** | mep8 |
