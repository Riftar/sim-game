# Neighborhood exterior layouts

[Places](places.json) describes four exterior layouts with market-event variants. [Catalog](catalog.json) describes the sixteen building exteriors and nine props supplied here. Use nearest-neighbor sampling. Some sample exteriors vary in width, wall height, and opening style. Use the size, anchor, footprint, and sockets for the exact variant you place.

Place an object's image at its position minus its catalog anchor. Objects use `[id,x,y]` tuples. For `new:` IDs look in this directory's catalog. For `existing:` IDs use the [original game object catalog](../objects/catalog.json). Use the sprite's sorting layer, footprint, and sockets for placement. All footprints and sockets are offsets from the anchor.

The route links connect named points in each layout. Use them as initial route and interaction markers. The event state changes sprite IDs at existing positions and adds props. The ordinary and event versions of the community hall have the same doorway and collision footprint.

- **Depok bakery lane** includes a pickup point for a bakery order or media side job.
- **Bekasi repair and reuse corner** includes a repair counter and a bank sampah sorting drop-off.
- **Manggarai balai warga courtyard** includes a hall entrance and a volunteer check-in area, with a market-event state.

- **Blok M Melawai strip** includes a fictional ramen ruko, thrift and record shop, creative venue, and MRT stair entrance. The creative-market state dresses the venue without shifting its doorway.

These layouts are asset data. Wire them into the game's map, collision, and mission systems when those systems are implemented.
