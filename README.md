# Safe Casing Surface STL Generator (Bmin–Bmax)

This script generates an **STL casing surface** around a **cylindrical magnet** by computing the magnetic-field magnitude **|B|** on a 3D grid and extracting the **threshold boundary** for a user-defined range:

**Bmin ≤ |B| ≤ Bmax**

The exported mesh represents the boundary surface(s) that enclose the region meeting that constraint.

---

## Output
Writes:
- `mag_band.stl` to `~/Documents/` (Windows/macOS/Linux)

On Windows, the script attempts to open File Explorer and highlight the STL after export.

---

## Requirements
Python 3.x and:
- `magpylib`
- `numpy`
- `scikit-image`
- `trimesh`
- `pyvista` (currently imported; not required unless you add visualization)

Install:
```bash
pip install magpylib numpy scikit-image trimesh pyvista
