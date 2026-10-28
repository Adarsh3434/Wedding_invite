# Ganesh N.D. & Arpitha M.R. — Wedding Invitation

A mobile-first, English-language wedding invitation with an interactive opening envelope, royal Indian burgundy-and-gold styling, countdown, family names, reception and ceremony details, gallery, map links, and background-music control. Sample wedding photographs are used until you provide your own.

## Wedding details currently configured
- **Couple:** Ganesh N.D. & Arpitha M.R.
- **Reception:** 19 November 2026, 7:00 PM
- **Wedding ceremony:** 20 November 2026, 6:00 AM
- **Venue:** Sri Jayadeva Veerashaiva Bhavaa, Nelmangala
- **Groom's parents:** Shubhashree & Dinesh
- **Bride's parents:** Mahadevi & M. N. Raju
- **Map:** https://maps.app.goo.gl/Q1KeapwZ2ze2ZKLm8?g_st=ic

## Run locally (Windows / VS Code)
1. Install Node.js LTS from https://nodejs.org/en/download
2. Extract this ZIP. Open the extracted folder that contains `package.json` directly in VS Code. There is no extra nested project folder in this ZIP.
3. Open Terminal → New Terminal. Run:
   ```powershell
   npm install
   npm run dev
   ```
4. Open the local address printed in the terminal (usually http://localhost:5173).
5. To verify the production build, run `npm run build`.

## Deploy to Netlify
- Import the project from a GitHub repository, or deploy the generated `dist` folder after running `npm run build`.
- Build command: `npm run build`
- Publish directory: `dist`
- Netlify's free plan and limits may change; check the current plan details.

## Change details and photos
- Edit names, date, family, event times, venue, map, and theme in `invitation.config.json`.
- Replace the sample image URLs in `src/modules/envelope/EnvelopeInteractive.tsx`, `src/modules/invitation/hero/HeroSection.tsx`, `src/modules/invitation/gallery/GallerySection.tsx`, and `src/modules/invitation/farewell/FarewellSection.tsx` with your own photos.
- The music player uses `src/assets/music/song.mp3`. Replace this with music you have permission to use if desired. Browsers may require the guest to tap the envelope or music button before playback.
- `index.html` contains social preview metadata. After deploying, replace the example `og:url` and Twitter URL with your actual Netlify URL.

## Before sharing with guests
Confirm the venue spelling and address, test the map link, and replace the sample photos/music with approved assets. The wedding countdown uses local browser time and targets 20 November 2026 at 6:00 AM.
