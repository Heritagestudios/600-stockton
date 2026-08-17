# 600 Stockton Street — 1919 Blender Reconstruction

## Model

This directory contains the first 3D reconstruction of the 1919
Metropolitan Life Insurance Company complex.

---

# Reconstruction Stage

Current stage:

**2D footprint → 3D massing**

The model will initially contain only:

- site
- building footprint
- courtyard/open space
- floor levels
- roof mass
- basic street context

Architectural ornament will be added only after the building massing has
been verified.

---

# Scene Organization

The Blender scene should eventually use the following collections:

```text
600_STOCKTON_1919
│
├── SITE
│
├── BUILDING
│   ├── FOOTPRINT
│   ├── MASSING
│   ├── COURTYARD
│   └── ROOF
│
├── ENVIRONMENT
│   ├── CALIFORNIA_STREET
│   ├── STOCKTON_STREET
│   └── PINE_STREET
│
├── EVIDENCE
│   ├── SANBORN
│   └── PHOTOGRAPHS
│
├── CAMERAS
│
└── LIGHTING
