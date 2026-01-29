# Moon Rocks - Status

*Last updated: January 28, 2026*

## Overview

A lunar rock collection game featuring a bouncy astronaut on the Moon. Touch/click to move the astronaut, collect moon rocks, and return them to the Lunar Module before oxygen runs out.

## Current State (v21) - Fully Playable

### Core Gameplay
- Astronaut follows finger/mouse with lunar bouncy physics
- Auto-collect rocks by running over them (unlimited carrying capacity)
- Deposit rocks at the Lunar Module (generous interaction zone - can slam-dunk while jumping over)
- Oxygen system drains while away from LM, refills when near
- Score based on rock rarity

### Rock Types (by rarity)
| Rock | Points | Rarity |
|------|--------|--------|
| Basalt | 10 | 50% |
| Anorthosite | 25 | 25% |
| Breccia | 50 | 15% |
| Orange Soil | 100 | 7% |
| Genesis Rock | 250 | 2.5% |
| Meteorite | 500 | 0.5% |

### Visual Features
- Detailed Apollo-style astronaut with articulated limbs
- Gold visor, blue/red suit connectors (from Apollo reference photos)
- Realistic lunar boots with ribbed soles
- Detailed Lunar Module with gold mylar, antennas, ladder, flag
- Parallax scrolling mountains
- Twinkling colored stars
- Earth in the sky
- Dust particles on jump/land
- Apollo-style footprints that appear on landing and fade over time

### Animation System (v44 base)
- Sine-based smooth hop animation
- Legs stay under body with slight alternating spread
- Arms swing opposite to each other
- Knees bend 35-70 degrees during hops
- Subtle body tilt (~4.5 degrees max)
- Direction only changes when on ground

### Sound Effects (Web Audio)
- Breathing noise (rhythmic)
- Rock pickup chime
- Lander arrival beep
- Rock deposit sound
- Alien gibberish speech

### UI/HUD
- Oxygen bar with warning colors (green/yellow/red)
- Carrying count
- Score display
- Lander direction arrow and distance
- **Oxygen warning at 55%** - Large animated "RETURN NOW" warning
- **Deposit HUD** - Visor-style manifest showing rocks deposited, sorted by total score, fades after 5 seconds

### Special Features
- **Aliens** - Cute lime green aliens (based on plush toy reference) spawn rarely in groups of 1-3, varying sizes, speak gibberish and run away when astronaut approaches
- **Rock highlighting** - Blue to purple glow on collectible rocks (within 300px)
- **Infinite terrain** - Rocks generate infinitely in both directions
- **Footprints** - Apollo-style ribbed bootprints appear on landing, fade over ~30 seconds

## Key Technical Details

### Animation Tuning (from extensive v33-v44 work)
```javascript
// Sine-based smooth animation
const hp = astro.hopProgress;
const spread = Math.sin(hp * Math.PI);

// Small leg separation, alternates each hop
const legSpread = spread * 0.12;  // ~7 degrees max

// Knees bend equally
const kneeBend = 0.6 + spread * 0.6;  // 35-70 degrees

// Arms swing opposite
```

### Finger tracking fix (critical bug fix)
```javascript
// Store SCREEN position, compute world position each frame
state.finger.screenX = x;  // On touch/mouse events
// Then each frame:
state.finger.x = state.finger.screenX + state.camera.x;
```

## Files

| File | Purpose |
|------|---------|
| `game.html` | Main game (v21) |
| `index.html` | Cache-busting redirect |
| `astronaut-mockup.html` | Original animation mockup (v44) |
| `reference/` | Apollo photos for boots, suits, footprints, lander |

## Run Instructions

```bash
cd ~/dev/game-ideas/moon-rocks && python3 -m http.server 8001
# Open http://localhost:8001
```

## Version History Highlights

- **v1-v2**: Basic game setup, rock collection, oxygen system
- **v3-v4**: Rock highlighting, positioning fixes
- **v5-v6**: Auto-collect, speed increase, high jump boost
- **v7-v8**: Infinite rock generation, slam-dunk deposits
- **v9**: Added alien character
- **v10**: Alien groups (1-3), blue/purple rock highlights, bigger aliens
- **v11**: Oxygen warning at 55%, deposit HUD with rock manifest
- **v12**: Sort HUD by total score per rock type
- **v13-v21**: Footprint system - Apollo-style ribbed prints, proper positioning, fade over time

## Known Issues (Fix Next Session)

1. **Oxygen drains too fast** - Make oxygen last longer
2. **Mobile portrait bug** - If player has finger on right side of astronaut and moves finger off screen to the right, astronaut launches fast to the LEFT (wrong direction)
3. **Mobile portrait scaling** - Astronaut looks huge on mobile in portrait mode
4. **Mobile landscape scaling** - Everything way too big, starts zoomed in with only top half of lunar lander visible
5. **Mobile finger controls** - Not enough space for finger, astronaut keeps getting too close to touch point causing control issues

**Root cause hypothesis:** Everything is just too big on mobile - fixing the scale might resolve most of these issues.

---

## What's Next (Ideas)

- More alien behaviors/interactions
- Rare special events
- Achievement system
- Different lunar locations
- Rover vehicle
