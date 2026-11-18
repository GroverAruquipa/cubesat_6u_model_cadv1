# TIGRE 4U/2U · Mechanical CAD

<p align="center"><img src="renders/stowed_6U.png" width="45%"> <img src="renders/pair_separated.png" width="45%"></p>

TIGRE is a two-body 6U CubeSat for the CSA CUBICS 2026 programme. It launches as a standard 6U and, in orbit,
separates into a **mother** (2x2U) and a **daughter** (2x1U) joined by a line. A winch in each body pays the line
out to 500 m and reels it back to 5 m.

| | |
|---|---|
| Mother | 200 x 100 x 227 mm, 4.00 kg |
| Daughter | 200 x 100 x 113.5 mm, 2.57 kg |
| Revision | Rev A, November 2026 |
| Author | Grover Aruquipa, Université Laval |

## Views

| Mother | Daughter | Winch |
|---|---|---|
| <img src="renders/mother_open.png" width="250"> | <img src="renders/daughter_open.png" width="250"> | <img src="renders/winch_module.png" width="250"> |

## Volume by subsystem

<p align="center"><img src="volumen_bloques.png" width="85%"></p>

Share of the volume taken by equipment in each body, from the solid volume of the CAD parts.

## Files

- `assembly/`: STEP assemblies of the stowed 6U, each body and the winch module
- `parts/`: every part as STEP and STL, sorted by body and subsystem
- `glb/`: models for web viewers
- `BOM_TIGRE_4U2U.xlsx`: mass of every part with its file name, and the purchased components with their datasheets

Part numbers follow `TGR-<body>-<subsystem>-<NNN>`, for example `TGR-M-WIN-009` (mother, winch, item 9).

## Notes

- Units in mm. Each body's origin is the centre of its separation face, with z pointing into the body.
- Parts are saved in place: importing all the files of a body rebuilds it without mates.
- No interferences, at least 0.5 mm of clearance between parts, and protrusions within the 6.5 mm CubeSat limit.
- Fasteners, connectors and harness routing are not modelled yet.

© 2026 Grover Aruquipa, Université Laval
