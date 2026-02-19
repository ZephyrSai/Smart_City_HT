# Smart City Digital Twin (Basemap + HT 3D)

This demo is now a digital-twin style 3D experience:

1. Basemap tiles are loaded and composited into a texture.
2. That texture is used as the ground/base plane in HT `Graph3dView`.
3. Buildings are superimposed as 3D blocks on top of the map base.
4. Clicking a building transitions to a separate building-only 3D view.
5. Use buttons to move between `3D City View` and `Building View`.
6. The dashboard is rendered as a glass-tinted overlay pane on top of the full-screen 3D map scene.
7. Map style can be switched in-app (Carto/OSM), with automatic fallback to OSM if a provider returns zero tiles.
8. Tile zoom level reloads dynamically based on camera distance (digital-twin style LOD behavior).

## Run

Open:

- `projects/smart-city-osm-3d/index.html`

## Notes

- Map attribution is shown in the UI and updates with style changes.
- Public tile usage has limits; for production, use compliant tile infrastructure.
- OSM tile policy: https://operations.osmfoundation.org/policies/tiles/
