# Figma Import Instructions – Findoc Design System

## Files Generated
- `figma-findoc-design-system.json` – Design System page (colors, typography, components)
- `figma-findoc-pages.json` – Auth and Dashboard page layouts (sample frames)

## How to Import into Figma

### Option A – Using a JSON Import Plugin
1. Install a JSON import plugin (e.g., “JSON to Figma”, “Figma JSON Importer”).
2. Open a new Figma file.
3. Run the plugin → choose `figma-findoc-design-system.json` first.
4. After import, rename the generated page to **01 Design System**.
5. Run the plugin again → choose `figma-findoc-pages.json`.
6. Rename the generated page to **02 Auth** and **03 Dashboard** as needed.

### Option B – Manual Recreation (if plugin unavailable)
Use the JSON as a spec:
- Create a **Design System** page.
- Add color swatches per the JSON (Primary 600, Ink 900, etc.).
- Create text styles (H1–H3, Body L/M/S, Label M).
- Build components (Button Primary/Secondary, Input, Stat Card, Status Chip).
- Create frames per the JSON coordinates and sizes.

## Validation Checklist

### Design System
- [ ] All 10 color swatches exist and match hex codes.
- [ ] Typography styles exist: H1 (48/700), H2 (36/700), H3 (28/600), Body L/M/S, Label M.
- [ ] Components created:
  - Button Primary (160×48, Primary 600 fill)
  - Button Secondary (160×48, Cloud 100 fill, Border 200 stroke)
  - Input Field (320×80, label + field + placeholder)
  - Stat Card (280×120, icon + label + value)
  - Status Chip (100×28, rounded 999px)

### Page Layouts
- [ ] Login Desktop frame: 1440×900, split layout, form card 400×500.
- [ ] Dashboard Desktop frame: 1440×900, top nav 72px, sidebar 260px, main content 1180px.
- [ ] All component instances reference the correct component IDs.
- [ ] Text content matches the spec (headings, labels, CTA copy).

### Interaction & Prototype Polish
- [ ] Create button hover variants (Primary → Primary/Hover).
- [ ] Add subtle hover glow on cards (use “Card / Elevated” component).
- [ ] Add tab interaction: Overview → Activity with smart animate.
- [ ] Link CTA buttons to Login/Signup frames for demo flow.
- [ ] Add a floating card in hero with slight scale (1.02) on hover.
- [ ] Use easing: `Smart Animate` + 200–300ms for micro transitions.

### Mobile Variants (to create manually)
- [ ] Create 390×844 frames for each page.
- [ ] Stack hero sections on Landing.
- [ ] Collapse sidebar to bottom nav on Dashboard.
- [ ] Convert tables to stacked cards.

## Next Steps
1. Import the JSON files via a plugin or recreate manually.
2. Add remaining pages (Document Detail, Upload/Verification, Admin Panel, Settings) using the same component library.
3. Create mobile variants by duplicating frames and adjusting layouts to 390×844.
4. Run a final audit: all colors, fonts, and components should be linked to the Design System page.

## Tips
- Use Auto Layout for responsive behavior.
- Pin elements to edges for proper constraints.
- Name layers clearly (e.g., “btn-primary”, “input-email”) for easier handoff.
- Export components as variants for hover/disabled states.

If you need me to generate additional page JSONs or a full mobile variant set, let me know!
