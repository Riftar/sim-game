# Game sprite assets

Use these transparent PNGs with nearest-neighbor sampling. Coordinates are in pixels, with Y increasing downward.

## Characters

[Character manifest](characters/manifest.json) lists five finished sprite sheets. Each sheet has four facing rows and 15 pose columns, with 96 × 144 texture pixels per frame. The frame occupies 32 × 48 world units. Place it relative to the ground pivot at [48, 132] texture pixels, or [16, 44] world units.

Use the manifest's direction and pose arrays to calculate the source rectangle. Each clip lists its sequence, frame durations in milliseconds, and loop behavior. Waiting and walking loop. Greeting and ticket-tap actions play once and end on idle. Move the actor separately through the game. Use the ticket-gate sprite from the object catalog as the scene prop.

The PNGs contain the final composited outfit for each character and the current prototype animation frames.

## Objects

[Object catalog](objects/catalog.json) lists 27 transparent sprites from the refined environment kit and transport trial. It includes buildings, plants, shop props, vehicles, station equipment, and weather and event decorations.

Position each object using its image anchor. Footprints and attachment sockets are relative to that anchor. A null footprint designates an object without blocking collision. Use the layer field to order ground, world, and overhead sprites. Transport footprints are starting values for map tests.
