# Geometry Detective

A self-contained interactive course demonstrator for task-sufficient geometry.

Live demo: https://li-wenzhan.github.io/geometry-detective-3dv/

## What the example demonstrates

The task is to retain enough positive surface evidence to identify the Chair category among a fixed aligned library of procedural Chair, Stool, and Wall shelf candidates.

1. Compare selection choices at the same point budget.
2. Compute an exact minimum over the fixed pool of 256 surface samples.
3. Remove each member of the complementary minimum pair and observe the competing category reappear.

Compatibility requires every retained point to lie within the fixed tolerance of a candidate surface. Distances use the boundary surfaces of the constituent axis-aligned cuboids, in normalized arbitrary units. The wireframe reference is display context, not additional retained evidence.

The exact minimum uses dynamic programming over the competitor-exclusion masks of all pool points. The lower-bound check also enumerates every singleton. This is a finite geometric identifiability result for the stated library, pool, alignment, and tolerance. It is not a learned classifier result, a recognition benchmark, or a universal point-count claim.

Open `index.html` directly for offline use, or serve this directory using any static HTTP server. Add `?stage=1` for the compact presentation view. The page uses no external libraries, network APIs, or user data collection.
