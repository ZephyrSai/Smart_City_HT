# Smart City Digital Twin (HT 3D + Map Basemap)

Interactive digital-twin proof of concept built with HT `Graph3dView`.

## What It Includes

- Full-screen 3D city world with map tiles composited as a ground texture.
- Dynamic map style switching (Carto Dark/Light/Voyager and OSM) with tile-source fallback.
- Zoom-aware tile reload based on camera distance for smoother detail transitions.
- Selectable buildings with telemetry-driven mock dashboards.
- Building detail view with popup metrics.
- RBAC mock roles (`Viewer`, `Operator`, `Admin`) controlling capabilities.
- Asset import workflow for `OBJ/MTL` and `FBX` model URLs.
- Editable layout mode to drag buildings, junctions, and imported assets.
- Route network + manually drawn road paths.
- Left live-alert glass rail and right dashboard panel.
- Resizable/collapsible side panels and collapsible top bar.

## Key Controls

- `3D City View` / `Enter Building View` / `Back To 3D World`
- `Map Style`
- `Set Map Center` (paste-friendly modal input)
- `Import Asset`
- `Road Path`
  - Turn on road draw mode.
  - Click scene points (building/junction/map surface) to add waypoints.
  - Click again to save the road path.
- `Edit Layout`
  - Drag movable objects while enabled.
- `Routes` toggle
- Sidebar controls
  - `Hide Alerts`, `Hide Dashboard`
  - Drag side resizers to change widths.
- `Collapse Top Bar`

## Run

Open:

- `projects/smart-city-osm-3d/index.html`

## Notes

- Attribution is shown in the UI and updates with selected map style.
- Public tile servers have usage limits; use compliant infrastructure for production.
- OSM tile policy: https://operations.osmfoundation.org/policies/tiles/
