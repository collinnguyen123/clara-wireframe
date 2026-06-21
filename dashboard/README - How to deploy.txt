clara — FULL SITE deploy bundle (homepage + dashboard in one link)
Built June 17, 2026.  REFRESHED June 21, 2026 (Session 31): added the full Migraine education section (Understanding, Treatments, Prevention & Triggers incl. the interactive Headache Diary), the new Neuropathic / Nerve pain education section (hub + PHN, Diabetic, CRPS, Fibromyalgia, Other Neuropathy), the Migraine Tracker, and refreshed the dashboard and homepage. All links re-verified: 35 pages crawl with zero broken references. Images capped at 1600px.

WHAT THIS IS
A single, self-contained website: the public landing page is index.html, and the
patient dashboard plus every education page, quiz, the cream/about/sign-in pages,
and the outcomes content are bundled alongside it. All links are relative and
verified — 25 pages crawl with zero broken references. Images capped at 1600px and
the two videos transcoded to ~0.9 MB each. Total ~149 MB.

THE TWO STATES (already wired)
- Logged out: open index.html (the landing page). The clara logo links to the
  landing page; the nav shows "Sign in"; no Dashboard link.
- Logged in: click the clara logo INSIDE the dashboard -> it returns to the landing
  page carrying ?signedin=1, and the nav now shows a "Dashboard" link that goes back
  inside. The signed-in state persists on the device (localStorage). To force the
  logged-out view again, open index.html?signedin=0

HOW TO PUSH IT LIVE (GitHub Desktop — the web uploader fails on large commits)
1. In Finder, open this "Deploy (full site)" folder and select ALL of its contents
   (index.html, the Clara-*.html files, and the asset folders).
2. Copy them into your repo folder:  Documents/GitHub/clara-wireframe/
   (Replace the existing files when prompted. Putting them at the repo ROOT makes the
   landing page the site root.)
3. Open GitHub Desktop -> review the changes -> Commit to main -> Push origin.
4. Wait ~1 minute for GitHub Pages to rebuild.

YOUR SHAREABLE LINK
   https://collinnguyen123.github.io/clara-wireframe/
   (Landing page. The dashboard is reachable from the nav once "signed in",
    or directly at .../clara-wireframe/Clara-Dashboard-MOCK-v1.html)

NOTE
This supersedes the older dashboard-only deploy that lived at
.../clara-wireframe/dashboard/. If you prefer to keep that path too, copy into a
subfolder instead of the root and tell Claude to adjust the links.
