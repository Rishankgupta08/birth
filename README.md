# A Little World for You — Birthday Surprise Website

A responsive, single-page birthday website with a cream, burgundy, blush-pink and antique-gold aesthetic to match the handmade QR card.

## Preview locally

Open `index.html` in a browser. An internet connection is only needed for the optional Google Fonts; the rest of the site is self-contained.

## Personalise before sharing

This is a starter draft. Please personalise it before making your QR code:

1. Replace generic phrases and the sample birthday letter with details that are true to your relationship.
2. Add your real photos to the six memory cards. In `index.html`, find each `<div class="photo-slot"> ... </div>` block and replace it with, for example:

   ```html
   <div class="photo-slot photo-filled">
     <img class="memory-img" src="assets/photo-1.jpg" alt="A favourite memory together">
   </div>
   ```

   Then add this CSS inside the `<style>` block:

   ```css
   .photo-filled { padding: 0; background: #f3dce0; }
   .memory-img { width: 100%; height: 100%; min-height: 270px; object-fit: cover; display: block; }
   @media (max-width: 800px) { .memory-img { min-height: 220px; } }
   @media (max-width: 480px) { .memory-img { min-height: 165px; } }
   ```

3. Put your images in the `assets` folder and make sure the filenames match the `src` paths.
4. Proofread every line; keep only details and promises you genuinely mean.
5. Deploy the folder to a public static hosting service such as Vercel or GitHub Pages. The QR code must point to the public deployed URL, not a local file path or `localhost`.
6. Scan the final printed QR code with another phone before giving the gift.

## Design

- Mobile-friendly one-page layout
- Interactive surprise cards
- Revealable final letter
- Small heart confetti on interactions
- No JavaScript libraries or build step required
