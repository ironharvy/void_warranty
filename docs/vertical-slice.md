# Vertical Slice

## Goal

Prove that the game is fun with one complete mission loop and minimal supporting systems.

The vertical slice should demonstrate:
- Vehicle handling.
- Boarding setup.
- Interior traversal.
- Objective retrieval.
- Escape pressure.
- Story framing and tone.

## Slice Mission

### Mission Name
Black Box Retrieval

### Premise
Alex is sent into a wrecked corporate vessel to recover a black box before a cleanup crew arrives. The mission is sold as routine salvage, but the recovered data becomes the inciting incident for the larger story.

## Player Flow

1. Mission briefing from employer.
2. Scripted docking / breach setup.
3. Vehicle deployment into the ship interior.
4. Navigation through 2 to 4 connected rooms or corridors.
5. Encounter one obstacle that rewards the correct vehicle choice.
6. Reach black box chamber and secure the objective.
7. Trigger alarm / collapse / defense escalation.
8. Escape to extraction point under pressure.
9. Return to base scene with Varrick or early story payoff.

## Scope Limits

The slice should include:
- One playable vehicle at first.
- Hook points for two additional vehicles.
- One enemy type plus one environmental hazard.
- One objective type.
- One extraction sequence.
- One short post-mission story scene.

The slice should not include:
- Open-ended space travel.
- Randomized ship layouts.
- Multiple factions.
- Crafting system.
- Large upgrade tree.
- More than one complete mission.

## Recommended Build Order

### Phase 1: Graybox Playability
- One test room.
- Basic vehicle controller.
- Camera and aiming readability.
- Pickup and extraction trigger.

### Phase 2: Mission Flow
- Scripted insertion.
- Objective room.
- Alarm state after pickup.
- End-of-mission success and failure states.

### Phase 3: Pressure
- Turret or drone defense.
- Timer or hazard escalation.
- Damage and destruction loop.

### Phase 4: Presentation
- Temporary UI.
- Audio cues.
- Mission briefing screen.
- Basic base scene and dialogue.

## Success Criteria

The slice succeeds if:
- Driving feels good within the first minute.
- The route is readable from the camera angle.
- The objective changes player behavior on pickup.
- Escape is meaningfully more tense than entry.
- The player understands the world and stakes without long exposition.

## Kill Criteria

Reassess the design if:
- Vehicle handling is not satisfying after repeated tuning.
- Interior readability breaks under the high-angle camera.
- The mission only becomes interesting through story, not mechanics.
- Too many systems are required before the first fun moment.
