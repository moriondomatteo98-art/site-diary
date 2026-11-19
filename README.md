# Site Diary

Transform Group daily site diary. Runs on GitHub Pages, stores data in Supabase (project `site-diary`, Sydney).

- `index.html` – the whole app
- `manifest.webmanifest`, `icons/` – home-screen app name and Transform icon
- `sw.js` – keeps the app on the phone so it opens with no signal (bump `VERSION` after changing any file)
- `lib/` – Supabase and jsPDF libraries, kept here so they work offline

Only the public (publishable) Supabase key is in the code. Row Level Security on every table and on the
private `photos` bucket means only the owner's account can read or write anything.
