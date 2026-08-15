# 600 Stockton Street — Sanborn Measurement Protocol

## Purpose

This document establishes the method used to extract measurable building
geometry from historic Sanborn Fire Insurance Maps.

The goal is to create a reproducible historical footprint dataset rather
than relying on visual approximation.

---

# Evidence Principle

Sanborn maps are treated as primary cartographic evidence.

Measurements extracted from the maps will be distinguished from:

- published architectural descriptions
- secondary-source measurements
- historically informed reconstructions
- visual estimates

No inferred measurement will be entered into the geometry dataset as
documented fact.

---

# Measurement Hierarchy

Measurements will be recorded in this order:

## 1. Explicit printed dimensions

If the Sanborn map directly labels a building dimension, that value has
the highest priority.

Example:

```text
60' or 80'
                 NORTH
                   ↑

                   Y+

                   │
                   │
WEST  ←────────────┼────────────→  EAST
                   │
                   │
                   │

                   Y-

             SOUTH / STOCKTON
Origin:
(0,0)

X-axis:
East / West

Y-axis:
North / South

Units:
Feet
Historic Sanborn PDF
        ↓
Identify correct sheet
        ↓
Locate 600 Stockton
        ↓
Identify printed scale/dimensions
        ↓
Measure footprint
        ↓
Calculate real-world dimensions
        ↓
Trace polygon
        ↓
Record coordinates
        ↓
Add to building-footprints.json
        ↓
Compare with photographs
