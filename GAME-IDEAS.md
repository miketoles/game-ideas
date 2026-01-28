# Game Ideas Collection

*Design concepts for future development*

---

## 1. Parkour Chill

### Core Concept
A zen side-scrolling parkour game where a nimble runner flows through procedural urban landscapes. No death, no pressure - just the satisfying rhythm of movement.

### The Feel
- **Flow state** - When you're in the zone, moves chain seamlessly
- **Stumble, don't die** - Bad timing = character stumbles, loses momentum, recovers
- **Style over speed** - Reward creative lines and move variety

### Controls

| Input | Action |
|-------|--------|
| Tap | Jump |
| Hold | Higher/longer jump |
| Swipe Up | Flip/vault |
| Swipe Down | Slide/roll |
| Touch wall | Wall-run (auto if close enough?) |

**Movement Options:**
- **Auto-run** (Alto's Odyssey style) - Player focuses purely on timing tricks
- **Speed control** - Drag left/right to control pace, allows more deliberate play
- **Hybrid** - Auto-run with brake/boost zones

### Moves & Mechanics

| Move | Trigger | Style Points | Notes |
|------|---------|--------------|-------|
| Basic Jump | Tap | 10 | Foundation |
| Precision Landing | Land on small platform | 25 | Tight timing |
| Wall Run | Touch wall while moving | 30 | Auto-grip, limited duration |
| Wall Jump | Tap during wall run | 40 | Chain multiple walls |
| Flip | Swipe up mid-air | 50 | Pure style |
| Vault | Swipe up near obstacle | 35 | Smooth over railings/AC units |
| Slide | Swipe down | 20 | Under obstacles |
| Roll | Swipe down on landing | 30 | Momentum recovery |
| Cat Leap | Jump to grab ledge | 45 | Climb up or swing |

### Combo System
- Chaining moves within ~1 second multiplies points
- Combo meter fills, multiplier increases: x2, x3, x4, x5 max
- Breaking flow (stumble, pause, repeat same move) resets combo
- "Perfect flow" bonus for long unbroken chains

### Stumble Mechanics (No Death)
Instead of dying:
- **Minor stumble** - Slight hesitation, lose combo
- **Big stumble** - Character trips, rolls, gets back up (2-3 sec recovery)
- **Fall** - Land on lower platform, climb back up or continue lower route

### Environment Generation

**Zones (procedural tiles):**
1. **Rooftops** - AC units, vents, gaps between buildings
2. **Scaffolding** - Metal beams, planks, hanging platforms
3. **Fire Escapes** - Zig-zag climbing, window ledges
4. **Construction Sites** - Cranes, beams, incomplete floors
5. **Alleyways** - Dumpsters, fences, narrow walls for runs
6. **Billboards & Signs** - Grab points, dramatic jumps

**Visual Progression:**
- Dawn/morning start (warm colors)
- Midday (harsh shadows, rooftop heat shimmer)
- Golden hour (long shadows, beautiful)
- Dusk/night (city lights, neon)

### Scoring & Progression
- **Run Score** - Total style points from one session
- **High Score** - Best ever
- **Achievements** - "Chain 20 moves", "100 flips total", etc.
- **Unlockables** - Character skins, trail effects, music tracks

### Audio
- Chill lo-fi beats or ambient electronica
- Footstep sounds match surface (gravel, metal, concrete)
- Whoosh sounds on flips
- Subtle crowd "ooh" on big moves

### Visual Style Options
- **Minimalist** - Simple shapes, bold colors (Monument Valley)
- **Pixel art** - Nostalgic, clear silhouettes
- **Stylized 3D** - Low-poly with nice lighting
- **Cel-shaded** - Comic book feel

### Inspiration
- Alto's Odyssey (zen flow, procedural, no death)
- Tony Hawk (combo chaining, style points)
- Mirror's Edge (first-person parkour feel)
- Canabalt (endless runner tension)

---

## 2. Rock Climber

### Core Concept
A meditative vertical climbing game. Control the climber's hands to ascend a massive wall - El Capitan or similar. Atmospheric, not punishing. The journey matters more than speed.

### The Feel
- **Meditative** - Slow, deliberate, contemplative
- **Physical** - Feel the strain, the relief of rest
- **Epic scale** - Tiny human vs massive wall
- **Atmospheric** - Weather, light, time passing

### Controls (Reuse Shipwreck Mechanic!)

**"Reach toward finger" adaptation:**
- Touch near a hand → that hand reaches toward your finger
- Drag to a hold → hand grabs it
- Release → hand stays gripped (or falls if no hold)

**Two-Hand System:**
| Touch Location | Action |
|----------------|--------|
| Left side of screen | Control left hand |
| Right side of screen | Control right hand |
| Near current hand | Fine adjustment |
| Far from hand | Big reach (uses more stamina) |

**Alternative: One-Hand-at-a-Time**
- Tap a hold → active hand reaches for it
- Tap different hold → switches which hand is active
- Simpler, might feel more natural

### Holds & Surfaces

| Hold Type | Grip Difficulty | Stamina Drain | Visual |
|-----------|-----------------|---------------|--------|
| Jug | Easy | Slow | Large, positive edge |
| Crimp | Medium | Medium | Small edge, fingers bent |
| Sloper | Hard | Fast | Rounded, friction-dependent |
| Pocket | Medium | Medium | Hole for 1-3 fingers |
| Crack | Varies | Medium | Jam hands/feet |
| Ledge | Rest spot | Recovers | Flat, can stand |

### Stamina System
- **Grip meter** per hand (or overall)
- Hanging drains stamina continuously
- Bigger reaches drain more
- Difficult holds drain faster
- **Rest positions:**
  - Ledges (full recovery)
  - Good stances (slow recovery)
  - Shake out (pause on jug, partial recovery)

**When stamina depletes:**
- Hand slips from current hold
- If both hands slip → fall to last checkpoint
- Not death, just setback

### The Wall: El Capitan Structure

**Vertical progression (bottom to top):**

| Section | Height | Character | Features |
|---------|--------|-----------|----------|
| Base | 0-500ft | Forest approach | Easy climbing, tutorial |
| Lower Wall | 500-1500ft | Steep granite | Learning real holds |
| Heart | 1500-2000ft | Famous features | Technical, exposed |
| Great Roof | 2000-2200ft | Horizontal section | Roof climbing mechanics |
| Upper Wall | 2200-2800ft | Varied terrain | Weather changes begin |
| Summit Push | 2800-3000ft | Final stretch | Dawn summit goal |

### Checkpoints & Bivouacs
- **Bivouac ledges** - Sleep overnight, full recovery, save point
- **Bolt anchors** - Quick checkpoint, brief rest
- **Notable features** - Named climbing landmarks

### Time & Weather

**Day/Night Cycle:**
- Climb during day, rest at night (or push through?)
- Light changes affect visibility, mood
- Sunrise/sunset at key moments

**Weather Events:**
| Weather | Effect | Vibe |
|---------|--------|------|
| Clear | Normal | Peaceful |
| Wind | Screen shake, harder reaches | Tense |
| Rain | Holds slippery, faster drain | Dangerous |
| Storm | Extreme, seek shelter | Dramatic |
| Fog/Cloud | Limited visibility, eerie | Atmospheric |
| Snow (high) | Cold damage?, icy holds | Summit push |

### Visual Design
- **Perspective** - Side view or slight 3/4 angle
- **Scale** - Climber is tiny, wall is vast
- **Detail gradient** - Close holds detailed, distant wall simplified
- **Parallax** - Multiple rock layers for depth

**Color Palette:**
- Granite greys with warm highlights
- Golden hour oranges
- Storm purples and greys
- Dawn pinks at summit

### Audio
- Ambient wind, birds, distant waterfalls
- Chalk bag sounds, rope rustling
- Breathing intensifies with stamina drain
- Music swells at achievements/vistas

### Progression
- **Main climb** - One massive El Capitan ascent
- **Routes** - Multiple paths up (easy tourist route vs hard direct)
- **Free solo mode** - No checkpoints, ultimate challenge
- **Achievements** - "Summit at sunrise", "No falls", etc.

### Inspiration
- Getting Over It (struggle, persistence)
- Celeste (challenge + kindness)
- Journey (atmosphere, scale)
- Real climbing documentaries (Free Solo, Dawn Wall)

---

## 3. Street Takeover

### Core Concept
Underground car culture meets arcade action. Burnouts, donuts, drifts, and sideshows. Build your garage, customize your rides, compete for pink slips. Win their car, take their pride.

### The Feel
- **Underground** - Nighttime, warehouses, empty intersections
- **Culture** - Car meets, spectator hype, reputation
- **Collection** - Build a garage of won cars
- **Style** - It's not just about winning, it's about HOW you win

### Core Mechanics

**Burnout:**
- Hold gas + brake, build RPM
- Release brake → tire smoke, noise, distance
- Score: duration × smoke density × straightness

**Donuts:**
- Tight circular spins
- Score: rotation count × tightness × consistency
- Perfect donut = tight circle, consistent radius

**Drifting:**
- Slide through corners
- Score: angle × speed × duration × proximity to walls

**Figure 8s:**
- Combine donuts in alternating directions
- Bonus for smooth transitions

### Controls

**Touch Controls:**
| Input | Action |
|-------|--------|
| Right thumb (low) | Gas |
| Right thumb (high) | Brake |
| Left thumb drag | Steering |
| Both thumbs + steer | Burnout/Donut initiation |

**Tilt option:** Steer with phone tilt, thumbs for gas/brake

### Competition Modes

| Mode | Rules | Win Condition |
|------|-------|---------------|
| Longest Burnout | Single run | Most distance/time |
| Donut Contest | 30 seconds | Highest rotation score |
| Drift Battle | Set course | Best drift score |
| Drag Race | 1/4 mile | Fastest time |
| Style Battle | Freestyle | Judge/crowd score |
| Figure 8 | Freestyle | Best figure 8 score |
| King of the Hill | Last car spinning | Outlast opponents |

### Pink Slip System

**Betting:**
- Put up your car against opponent's car
- Winner takes both (or just opponent's)
- Risk/reward: Better cars = harder opponents

**Garage Building:**
- Start with beater
- Win cars, build collection
- Sell duplicates for upgrade cash
- "Stable" of different cars for different events

### Car Customization

**Performance:**
| Category | Upgrades | Effect |
|----------|----------|--------|
| Engine | Intake, headers, turbo, supercharger | More power |
| Tires | Compound, width, brand | Grip, burnout smoke |
| Suspension | Coilovers, sway bars | Handling, stance |
| Transmission | Short throw, gear ratios | Acceleration |
| Differential | LSD, welded | Donuts, drifting |
| Weight | Strip interior, cage | Power/weight |

**Visual:**
| Category | Options |
|----------|---------|
| Paint | Colors, metallics, mattes, wraps |
| Wheels | Styles, sizes, offsets |
| Stance | Ride height, camber |
| Body | Kits, spoilers, lips |
| Lights | Headlights, underglow |
| Interior | Roll cage, seats, gauges |

### Car Classes

| Class | Examples | Character |
|-------|----------|-----------|
| JDM | Silvia, Supra, RX-7 | Drift kings |
| Muscle | Mustang, Camaro, Charger | Burnout beasts |
| Euro | M3, Golf R, RS4 | All-rounders |
| Lowrider | Impala, Monte Carlo | Show style |
| Truck | Silverado, F-150 | Burnout monsters |
| Exotic | 911, Corvette | Pink slip trophies |

### Locations

**Sideshow Venues:**
1. **The Intersection** - Classic takeover spot, 4-way
2. **The Warehouse District** - Long straights, corners
3. **The Bridge** - Dramatic backdrop, echo acoustics
4. **The Mall Lot** - Wide open, late night
5. **The Waterfront** - Scenic, spectator-friendly
6. **The Industrial Yard** - Gritty, underground feel

### Spectator System

**Crowd Mechanics:**
- NPCs gather to watch
- Hype meter builds with good moves
- Crowd goes wild = bonus points
- Spectators record on phones (visual flair)
- "That's going viral!" moments

**Reputation:**
- Build rep through events
- Higher rep = bigger crowds, better opponents
- Rep unlocks exclusive events, cars

### Multiplayer Potential

**Async:**
- Ghost battles (compete against recorded runs)
- Leaderboards per event type
- Weekly challenges

**Real-time (future):**
- Head-to-head drag
- Drift battles
- Crew vs crew sideshows

### Audio
- Engine sounds per car (V8 rumble vs inline-4 scream)
- Tire screech, rubber burning
- Crowd noise, air horns, cheering
- Hip-hop/trap soundtrack
- "OH!" reactions on big moves

### Visual Style
- **Time of day** - Mostly night, streetlights, headlights
- **Smoke** - Thick, volumetric tire smoke
- **Camera** - Dynamic angles, drone shots, spectator POV
- **Effects** - Sparks, rubber marks, heat shimmer

### Progression Loop
1. Start with beater car
2. Enter low-stakes events
3. Win, upgrade, or win new car
4. Enter higher-stakes events
5. Build garage collection
6. Become legend of the scene

### Inspiration
- Midnight Club (car culture, customization)
- Need for Speed Underground (tuner scene)
- Real sideshow culture (YouTube)
- Car meet Instagram aesthetic

---

## 4. Moon Rocks

### Core Concept
Apollo-era lunar exploration. Drive a rover across the moon's surface, hop out to collect rock samples, return them to the lunar lander. Manage your oxygen. A love letter to the space program with a 1960s/70s NASA aesthetic.

### The Feel
- **Wonder** - The loneliness and beauty of the lunar surface
- **Exploration** - What's over that next ridge?
- **Retro-futurism** - Kennedy-era optimism, analog gauges, crackly radio
- **Gentle tension** - Oxygen awareness without panic
- **Americana** - Little flag by the lander, "one small step" vibes

### Core Loop
1. Start at lunar lander (home base)
2. Get in rover, drive out exploring
3. Spot interesting rocks, stop rover
4. Get out, walk to rocks, collect samples
5. Get back in rover, continue or return
6. When rover cargo full OR oxygen getting low → return to lander
7. Deposit samples, refill oxygen, go again

### Controls

**Rover Mode:**
| Input | Action |
|-------|--------|
| Touch right side | Accelerate |
| Touch left side | Brake/reverse |
| Tilt or drag | Steering |
| Tap astronaut icon | Exit rover |

**On Foot Mode:**
| Input | Action |
|-------|--------|
| Touch/drag | Walk toward finger (Shipwreck-style!) |
| Tap rock | Collect sample |
| Tap rover | Enter rover |
| Near lander | Auto-deposit, refill O2 |

### The Astronaut

**Visual Design (1960s Apollo style):**
- Bulky white EVA suit (grey/white monochrome palette)
- Dark visor on helmet (side-view, faces direction of movement)
- Portable Life Support System (PLSS) backpack with hoses
- Articulated limbs (hip/knee, shoulder/elbow joints)
- Puffy suit segments with joint rings
- Moon boots with flat soles and tread marks

**Movement Feel - IMPLEMENTED IN MOCKUP:**
- **Finger height controls hop intensity!**
  - Touch HIGH on screen = big floaty Apollo bounds (up to 5x intensity)
  - Touch LOW on screen = quick little bunny hops (down to 0.25x intensity)
- Bounding gait with alternating feet (not bunny hop with legs together)
- Push-off motion - back leg extends to push, front leg reaches down to land
- Body leans into movement direction
- Squash on landing, stretch at apex
- Direction only changes when on ground (prevents mid-air glitching)

**Animation System (2.5D side-view):**
- `facingRight` with `flipProgress` for smooth turn transitions
- Scale X through 0 for 2.5D flip effect
- Layered drawing: back leg → back arm → PLSS → torso → front leg → front arm → helmet
- `hopProgress` tracks animation phase (0 = push-off, 1 = landing)
- `hopVariation` randomizes each hop (0.25x to 5x based on finger height + small random)
- `hopSpeedVar` makes bigger hops floatier, smaller hops snappier

**Organic Variation (like Apollo footage):**
- Random slight variation in hop strength each bounce
- Arm wobble - slight random adjustment each hop
- Body squash/stretch - compresses on landing, stretches at apex
- Dynamic dust - more particles for harder landings
- Shadow scales with height
- Idle breathing/sway animation when standing still

**Dust & Footprints:**
- Dust particles on push-off and landing
- Intensity scales with hop strength and landing velocity
- Footprints left in regolith
- Dust falls slowly (moon gravity on particles too)

### The Lunar Rover (LRV)

**Visual Design:**
- Wire-frame wheels (real Apollo design)
- Open chassis, no roof
- Antenna dish
- Camera on front
- Sample bags mounted on back
- Orange fenders over wheels

**Driving Feel:**
- Bouncy suspension over terrain
- Dust rooster-tail behind
- Top speed ~8 mph (realistic) or faster for fun?
- Can tip over on steep slopes (astronaut tumbles out, recovers)

**Cargo System:**
| Capacity | Rocks |
|----------|-------|
| Rover bed | 6-8 samples |
| Astronaut (on foot) | 1-2 samples |

### Oxygen System

**The Meter:**
- Always visible in corner
- Starts at 100%
- Drains slowly while on foot
- Pauses while in rover (suit connected to rover supply)
- Pauses at lander (unlimited supply)

**Drain Rates:**
| Activity | Drain Rate |
|----------|------------|
| Walking | Normal |
| Running/hopping | Faster |
| Standing still | Slower |
| In rover | Paused |
| At lander | Refilling |

**Low Oxygen:**
- Warning beeps at 25%
- Screen edges tint red at 15%
- At 0% = mission over, return to lander

**Philosophy:** Tension, not punishment. Plenty of time to return if you pay attention. Encourages planning: "How far can I go and still get back?"

### Rock Types & Scoring

| Rock Type | Points | Rarity | Visual | Location |
|-----------|--------|--------|--------|----------|
| Basalt | 10 | Common | Dark grey | Everywhere |
| Anorthosite | 25 | Common | Light grey/white | Highlands |
| Breccia | 50 | Uncommon | Mixed texture | Crater rims |
| Orange Soil | 100 | Rare | Orange tint | Volcanic areas |
| Genesis Rock | 250 | Very Rare | Crystalline white | Deep craters |
| Meteorite | 500 | Ultra Rare | Black, metallic | Random |

### Terrain Features

**Surface Types:**
- **Mare (seas)** - Flat, dark basalt plains, easy driving
- **Highlands** - Lighter, rougher, more interesting rocks
- **Regolith** - Fine dust everywhere, tracks visible behind rover

**Landmarks:**
| Feature | Gameplay | Visual |
|---------|----------|--------|
| Craters | Steep edges, rare rocks in center | Bowl shapes, various sizes |
| Boulders | Obstacles, sometimes climbable | Large rocks, shadows |
| Rilles | Channels to drive along/across | Long valleys |
| Hills/ridges | Block view, rewards for climbing | Rolling terrain |
| Small craters | Bumps to drive over | Pockmarks everywhere |

### The Lunar Lander (Home Base)

**Visual Design:**
- Apollo Lunar Module style
- Gold foil, silver legs
- Descent stage (base)
- American flag planted nearby
- Footprints around it
- Earth visible in black sky above

**Functions:**
- Deposit collected rocks (score tallied)
- Refill oxygen (instant or animated?)
- Save point / session checkpoint
- "Home" marker always visible on HUD

### Visual Style: 1960s/70s NASA Aesthetic

**Color Palette:**
| Element | Color | Hex |
|---------|-------|-----|
| Lunar surface | Grey-tan | #C4B8A8 |
| Shadows | Deep grey | #2A2A2A |
| Sky | Pure black | #000000 |
| Earth | Blue marble | #4A90D9 |
| Stars | White dots | #FFFFFF |
| Suit | Off-white | #F5F5F0 |
| Rover | Silver/grey | #A8A8A8 |
| LM gold foil | Gold | #D4AF37 |
| Flag | Red/white/blue | USA colors |

**Visual Effects:**
- No atmosphere = stark shadows, no haze
- Footprints and tire tracks persist
- Dust particles when moving
- Lens flare from sun?
- Film grain overlay option (period authentic)
- CRT scan lines option

**UI Style:**
- NASA mission control aesthetic
- Green phosphor text option
- Analog gauges (O2 meter as round dial)
- Mission elapsed time counter
- Coordinates display
- Crackly radio font

### Audio

**Ambient:**
- Silence of space (most of the time)
- Suit breathing sounds
- Heartbeat when O2 low
- Radio static/crackle

**Sound Effects:**
- Crunchy regolith footsteps
- Rover motor whine
- Rock pickup "clunk"
- Airlock hiss at lander
- Beeps and boops (Apollo computer style)

**Music:**
- Minimal during gameplay (preserve loneliness)
- Triumphant orchestral on big discoveries
- 60s space-age music in menus?
- Strauss "Blue Danube" vibes

**Radio Chatter:**
- Occasional Houston comm (text + audio crackle)
- "Looking good, 12" style callouts
- Congratulations on rare finds

### Exploration & Distance

**Map Structure:**
- Lander at center
- Infinite (or very large) terrain in all directions
- Procedurally generated but seeded (same world each session)
- Distance from lander tracked

**Distance Tiers:**
| Range | Character | Risks |
|-------|-----------|-------|
| 0-500m | Safe zone | Easy return, common rocks |
| 500m-2km | Exploration | Good rocks, watch O2 |
| 2-5km | Far out | Rare rocks, careful planning |
| 5km+ | Expedition | Best finds, real commitment |

**Navigation:**
- Compass showing lander direction
- Distance to lander readout
- Tire tracks to follow back
- Landmarks to memorize

### Progression & Scoring

**Session Score:**
- Total points from deposited rocks
- Bonus for variety (collected all types)
- Distance traveled bonus
- Efficiency bonus (rocks per O2 used)

**Persistent Progress:**
- Total rocks collected (lifetime)
- Rarest finds catalog
- Furthest distance reached
- Achievements

**Achievements:**
- "First Steps" - Walk 100m from lander
- "Geologist" - Collect one of each rock type
- "Long Drive" - Travel 5km in one expedition
- "Close Call" - Return with <5% oxygen
- "Motherlode" - Fill rover completely with rare rocks
- "Giant Leap" - Travel 10km from lander

### Session Flow

**Typical 10-minute session:**
1. Start at lander, full O2
2. Drive out ~1km, spot crater
3. Park rover, walk to crater rim
4. Collect 3-4 rocks, O2 at 60%
5. Return to rover, drive further
6. Find interesting boulder field
7. Collect more, O2 at 30%
8. Drive back to lander
9. Deposit ~8 rocks, refill O2
10. Check score, maybe go again or end

### Open Questions

- **Rover speed:** Realistic (8mph) or faster for fun?
- **Oxygen strictness:** How much buffer time?
- **Rover tipping:** Funny inconvenience or actual problem?
- **Night cycle:** Does moon rotate? Dark side exploration?
- **Landmarks:** Procedural or hand-placed points of interest?
- **Multiplayer:** See other astronauts' footprints/rovers?

### Inspiration
- Apollo mission footage and photos
- For All Mankind (TV show aesthetic)
- Lunar Lander (classic game)
- Desert Bus (meditative driving)
- Death Stranding (lonely exploration, cargo management)
- Real Apollo 15-17 rover footage

### Implementation Status

**Astronaut Animation Mockup - COMPLETE**
- File: `/Users/miketoles/dev/game-ideas/moon-rocks/astronaut-mockup.html`
- Reference: `/Users/miketoles/dev/game-ideas/moon-rocks/reference/` (Apollo footage gifs)
- Run: `cd ~/dev/game-ideas/moon-rocks && python3 -m http.server 8001`

**What's Working:**
- Finger-puppeted movement (touch left/right to walk)
- Finger height controls hop intensity (core mechanic!)
- 2.5D side-view with smooth flip transitions
- Articulated limbs with proper bounding gait
- Organic variation in each hop
- Body squash/stretch on landing/apex
- Dynamic dust particles
- Lunar lander, flag, parallax mountains, starfield
- Monochrome grey/black/white Apollo aesthetic

**Next Steps:**
- Add lunar rover
- Add rock collection mechanic
- Add oxygen system
- Expand terrain

---

## Quick Comparison

| Aspect | Parkour Chill | Rock Climber | Street Takeover | Moon Rocks |
|--------|---------------|--------------|-----------------|------------|
| Orientation | Horizontal | Vertical | Top-down/3rd person | Horizontal side-scroll |
| Core input | Timing taps | Drag to holds | Gas/brake/steer | Drive + walk to finger |
| Vibe | Flow state | Meditative | Hype/competition | Wonder/exploration |
| Progression | High scores | Summit goal | Car collection | Rock catalog |
| Fail state | Stumble | Fall to checkpoint | Lose car/event | Run out of O2 |
| Multiplayer | Leaderboards | Ghost climbs? | Head-to-head | Shared footprints? |

---

## Open Questions

### Parkour Chill
- Auto-run or player speed control?
- How to make procedural feel hand-crafted?
- Endless or level-based?

### Rock Climber
- One-hand or two-hand control?
- How punishing should falls be?
- Multiple routes or one epic climb?
- Real El Capitan or fictional wall?

### Street Takeover
- How realistic vs arcade physics?
- Pink slip economy balance (don't lose everything)
- Single-player depth vs multiplayer focus?

### Moon Rocks
- Rover speed: realistic (8mph) or faster for fun?
- Oxygen strictness: how much buffer time?
- Rover tipping: funny inconvenience or real problem?
- Night cycle: dark side exploration?
- Landmark generation: procedural or hand-placed?

---

## Development Priority Thoughts

**Easiest to prototype:** Parkour Chill (2D, simple physics)
**Most unique mechanic:** Rock Climber (finger-following hands)
**Biggest scope:** Street Takeover (cars, customization, multiplayer)
**Most atmospheric:** Moon Rocks (strong visual identity, clear gameplay loop)

**Reusable from existing games:**
- Shipwreck finger-following → Rock Climber hands, Moon Rocks astronaut walking
- Shipwreck boat/diver relationship → Moon Rocks lander/astronaut
- Bulldozer flip animation → Parkour character turns
- Bulldozer vehicle controls → Moon Rocks rover driving
- General 2D physics → Parkour, Rock Climber, Moon Rocks

---

*Ideas waiting to become reality.*
