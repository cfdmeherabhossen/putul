# For Putul, with love ♡

A responsive, single-file romantic proposal website. Open `index.html` in a modern browser; no installation or build step is needed.

## Personalize it

Search `index.html` for these comments:

- `EDIT HER NAME AND YOUR INTRO TEXT HERE`
- `EDIT HER PHOTO HERE` — the three supplied JPEG photos are embedded directly in the HTML in the order provided. Replace an image’s `src` and `alt` text to change a photo.
- `EDIT HER FAVORITE BEHAVIOR HERE`
- `EDIT QUIZ QUESTIONS / OPTIONS HERE`
- `EDIT YOUR PROPOSAL QUESTION HERE`
- `EDIT YOUR POP-UP LOVE NOTE AND SIGNATURE HERE`
- `EDIT HER PROFILE LINK HERE`

All three supplied photos are included as original JPEG data URIs, with no separate image files or external photo host. The gallery preserves each full picture, including the collage, without cropping. The envelope illustration is built entirely with inline SVG and CSS.

## Interactions

- Pick one favorite photo; the selection survives a reload when browser storage is available.
- Enter comfort food, choose a date, and add an optional wish. “Keep this little plan” saves on the current device.
- Choose **YES! ❤️** to open the love note and launch canvas-confetti. Current quiz answers personalize the note.
- **No 🙈** makes one small mouse-only dodge and remains fully clickable. Touch, keyboard, and reduced-motion users can choose it directly.
- Close the note with its close button, the bottom button, Escape, or a click outside it. Keyboard focus returns to YES.

There is no backend, analytics, or answer submission. Photo choices and saved quiz answers stay in this site's browser storage. The yes response is not sent or persisted. The page asks search engines not to index it; this is not an access restriction.

## Host it

### GitHub Pages

In this repository, open **Settings → Pages**, choose **Deploy from a branch**, select **main** and **/ (root)**, then save. The intended URL is `https://cfdmeherabhossen.github.io/putul/` once Pages is enabled and its deployment succeeds.

### Netlify

Drag a folder containing `index.html` into Netlify's deploy interface, or connect this repository with no build command and the repository root as the publish directory.

## Dependencies

Application HTML, CSS, and JavaScript live in one file. Tailwind CSS loads from its browser CDN, canvas-confetti from jsDelivr, and fonts from Google Fonts. These external assets require an internet connection; the embedded gallery photos do not. The custom CSS preserves the layout if Tailwind is unavailable, and the love note works even if confetti cannot load.

References: [Tailwind CDN](https://tailwindcss.com/docs/installation/play-cdn), [canvas-confetti](https://github.com/catdad/canvas-confetti).
