# AI-Assisted Pipeline

## Principle

AI should accelerate production, not define the game by itself. Use AI to reduce drafting time, placeholder creation time, and repetitive implementation work. Keep final decisions on feel, scope, and style under manual control.

## Best Uses For AI

### Design And Writing
- Turn rough ideas into structured specs.
- Draft mission briefings, comms chatter, codex entries, and ad copy.
- Generate alternate quest setups and progression ideas.
- Run consistency checks against the world bible.

### Code
- Generate small Unity components with clear responsibilities.
- Draft editor tools, mission data assets, and debug utilities.
- Produce test plans and regression checklists.
- Refactor repetitive gameplay code after the design stabilizes.

### Art Pre-Production
- Create moodboards.
- Explore silhouettes for vehicles and ship interiors.
- Generate signage, ads, decals, and UI concept art.
- Produce rough prop concepts for later modeling.

### 3D Asset Prototyping
- Use tools like Meshy for rough salvage props, debris, cargo, and background objects.
- Use image-to-3D as a starting point, not the finish line.
- Clean up or replace assets that break silhouette readability or camera clarity.

## Poor Uses For AI

- Finalizing core gameplay feel.
- Designing camera behavior without testing.
- Generating all major hero assets without cleanup.
- Producing final UI with no human visual direction.
- Making architecture decisions through giant prompts.

## Recommended Tool Roles

### Codex / ChatGPT / Claude
- Design docs.
- Unity scripts.
- Data model definitions.
- Content generation.
- Debugging assistance.

### Image Models
- concept art.
- mission key art.
- in-world ad campaigns.
- interface styling.

### Meshy Or Similar
- rough props.
- salvage items.
- industrial clutter.
- early environment kit pieces.

### Blender
- Cleanup pass for generated geometry.
- Retopology or simplification when needed.
- Pivot correction, scaling, and collision planning.

## AI Asset Rules

Use AI-generated assets first for:
- Crates.
- Containers.
- Debris.
- Wall machinery.
- Salvage pickups.
- Disposable decorative props.

Avoid depending on AI-first assets for:
- The player's main vehicle.
- The most common vehicle silhouettes.
- Any asset that requires high-quality animation.
- Core interaction-heavy objects seen up close for long periods.

## Workflow For AI-Generated Props

1. Generate concept image or 3D draft.
2. Evaluate silhouette at gameplay camera distance.
3. Clean model in Blender if needed.
4. Standardize scale and pivot.
5. Create simple collision.
6. Apply unified material treatment in Unity.
7. Test against the actual camera and lighting.

## Legal And Production Note

Track which assets are AI-generated, store source prompts or source images when practical, and keep replacement flexibility. Do not build the project's identity around assets you cannot confidently ship or revise later.
