# Repzy landing page

A small React + Vite site, separate from AI_GYM_TRAINER.

## Run

Requires Node.js 22.13+.

```powershell
npm install
npm run dev
```

Open http://127.0.0.1:5173. Run the Streamlit trainer separately on port 8501.

## Files you edit

- `src/App.jsx`: page content, gallery image URLs and trainer buttons.
- `src/styles.css`: colours, layout and responsive styling.
- `src/main.jsx`: React entry point.
- `public/favicon.svg`: site icon.
- `index.html`: title and description.
- `vite.config.js`: local development and preview settings.

## Trainer URL

Copy `.env.example` to `.env.local` and change `VITE_TRAINER_URL` if needed. Restart or rebuild after changes. For a public deployment use your hosted trainer URL, not localhost. Existing NEXT_PUBLIC_TRAINER_URL settings were migrated during the conversion.

## Build

`npm run build` creates `dist/`. `npm run preview` serves that production build locally on http://127.0.0.1:4173.

`node_modules/` is installed dependencies; `dist/` is generated output. Both are ignored by Git. No Next.js, Cloudflare, Sites runtime, TypeScript or Tailwind setup is required.

## Photography

The hero photograph loads from Unsplash and requires internet access. The three gallery illustrations are generated assets stored locally in public/images/. They explain angle detection, rep counting and form feedback; they are not actual app screenshots. The original trainer application is unchanged.


## Generated gallery assets

Created with the built-in image-generation tool. Final prompts:

### angle

Use case: scientific-educational. Create a premium gym AI feature illustration, square 1024x1024. Photorealistic adult athlete in black workout clothes, side-on, waist-up in a charcoal gym. Biceps curl midway: upper arm vertical, forearm horizontal, anatomically plausible elbow at 90 degrees. Crisp orange #f07a45 tracking lines connect visible shoulder, elbow, wrist, three bright circular joint markers precisely aligned, angle arc at elbow. Minimal white typography 'ELBOW ANGLE' and '90°'. Small bottom label 'FEATURE ILLUSTRATION'. Dark steel background, professional sports photography, clear arm silhouette, ample safe margins. This illustrates pose estimation, not an actual screenshot. No green, no fake accuracy claims, no extra limbs, no logos, no browser frame.

### reps

Use case: ui-mockup. Create a premium gym AI feature illustration, square 1024x1024. Photorealistic adult woman in charcoal workout clothing, full body side-on just standing upright after a bodyweight squat, in dark gym. Orange #f07a45 thin pose-estimation skeleton connects shoulder hip knee ankle precisely over visible body with circular joint markers. A restrained dark compact readout beside athlete in large legible white text 'REPS 08' and smaller 'RETURN COMPLETE'. Small bottom label 'FEATURE ILLUSTRATION'. Show exactly one athlete, clear limbs head and shoes within frame, realistic sports photograph, dark steel black backdrop, orange accents matching companion elbow-angle visualization. No browser chrome, no green, no accuracy claims, no extra limbs.

### feedback

Use case: scientific-educational. Create a premium gym AI feature illustration, square 1024x1024. Photorealistic adult athlete side-on doing a standing dumbbell curl in a dark gym; elbow slightly drifting forward away from torso, upper arm inclined forward. Bright orange #f07a45 pose-estimation points precisely on shoulder elbow wrist hip joined by thin lines. A subtle orange directional arrow at elbow points back toward torso to illustrate a correction. Minimal compact dark feedback card with perfectly readable white text 'FORM FEEDBACK' and 'Keep your elbow near your torso'. Small bottom label 'FEATURE ILLUSTRATION'. Black steel and orange palette, elegant professional sports photograph, anatomically plausible body and grip, ample margins, one athlete. Educational conceptual graphic, not a real app screenshot. No green, no fake scores, no extra limbs, no browser chrome.
