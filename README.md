# Signal City

A single-intersection Three.js traffic control arcade game. Serve `dist/` from localhost with `python3 -m http.server 8000 --directory dist`, then open `http://localhost:8000`. A hosted HTTPS version can be published once source synchronization is available. The game loads Three.js and its UI font from CDN.

## Mac browser validation

Run the deployed HTTPS page in current Safari and Chrome on the target Mac. Allow location once, then repeat with location denied and select a fallback city/time. For each browser:

1. Orbit and zoom. Confirm signals, moving cars, crossings, shadows, and readable controls at several angles.
2. Run a non-peak round and a peak round. Confirm peak mode creates visibly denser queues, cars stop at red, pedestrians wait for WALK, and throughput increments.
3. Set conflicting vehicle greens, then vehicle and pedestrian conflicting greens. Confirm the safety count rises and score drops. Restart and finish a full three-minute round.
4. Compare Auto, High, Medium, and Low graphics. Note FPS displayed by the game, visual artifacts, heat/fan behavior, and whether controls remain responsive in peak mode.
5. Resize the browser and check the narrow layout. On a phone-width view, tap the Signal City heading to swap between the signal board and score panel.

Record Mac model, macOS version, browser versions, resolution, FPS range in peak mode, and any screenshots of visual defects. Expand the city only after both browsers meet the agreed visual and performance target.

## Controls

Drag to orbit; scroll to zoom. Use signal board controls to set each vehicle approach or pedestrian crossing to RED, AMBER, GREEN, WAIT, or WALK. Conflicting greens are permitted and penalized. Select peak mode before or during a shift. Settings provide location, city/time fallback, and graphics override.
