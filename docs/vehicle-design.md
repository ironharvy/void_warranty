# Vehicle Design

## Design Rules

- Each vehicle must solve a different traversal or combat problem.
- Vehicle readability matters more than realism.
- The player should understand the role of each vehicle in seconds.
- A mission should reward choosing the right vehicle without hard-failing unusual playstyles.

## Vehicle 01: Runner

### Purpose
Fast insertion, objective retrieval, route scouting.

### Strengths
- Highest speed.
- Tight turning radius.
- Fits through narrow ship corridors.

### Weaknesses
- Low armor.
- Weak against turrets and drones.
- Limited ability to force through obstacles.

### Design Notes
This is the best first vehicle for the vertical slice because it makes route readability and extraction pacing obvious. It also fits the "steal and run" fantasy at the center of the game.

## Vehicle 02: Breaker

### Purpose
Heavy breach unit for contested routes.

### Strengths
- High armor.
- Strong ram or breach capability.
- Best against fixed defenses.

### Weaknesses
- Slow acceleration.
- Large silhouette.
- Struggles in narrow spaces and timed escapes.

### Design Notes
Breaker creates route tradeoffs. It opens paths that Runner cannot safely handle, but it increases extraction risk if speed matters.

## Vehicle 03: Skimmer

### Purpose
Hover-based utility vehicle for unstable and vertical spaces.

### Strengths
- Can cross gaps or unsafe floor sections.
- Better mobility over hazards.
- Useful for reactor rooms and broken hull areas.

### Weaknesses
- Medium durability.
- Lower direct force than Breaker.
- More tuning complexity than the other vehicles.

### Design Notes
Skimmer should be added after the vertical slice proves itself. It expands mission variety but is not necessary to validate the main loop.

## Initial Upgrade Slots

To keep progression manageable, vehicles should share a small modular upgrade framework:
- Armor slot.
- Utility slot.
- Mobility slot.

Example modules:
- Reinforced plating.
- Short-burst jammer.
- Cargo clamp stabilizer.
- Emergency repair charge.
- Overdrive boost.

## First Vehicle Recommendation

Start production with Runner only.

Reasons:
- Simplest control profile.
- Best fit for the first black box mission.
- Puts emphasis on movement and extraction tension.
- Avoids balancing three vehicles before the loop is proven.
