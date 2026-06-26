clara — FULL SITE deploy bundle
Rebuilt 2026-06-26 (Session 37 deploy).  ~510 MB, 23 top-level pages + education + trackers + provider portals.

================================================================
WHAT THIS BUNDLE IS
================================================================
One self-contained website covering the ENTIRE wireframe so it can be shared with anyone:

PATIENT / PUBLIC (logged-out marketing site)
  index.html ................... landing page (= Clara-Homepage)
  Clara-Homepage / KneePain / BackPain / Migraine / NervePain
  Clara-TheCream / HowItWorks / YourPlan / AboutUs
  Clara-SignIn ................. patient sign in / sign up
  the four assessment quizzes (Knee, Back, Migraine, Neuropathic)

PATIENT (logged-in experience)
  Clara-Dashboard .............. the patient dashboard
  Pain Tracker, Migraine Tracker, daily/monthly/quarterly check-ins
  all 16 education pages (Knee OA, Low Back, Migraine, Neuropathic)

PROVIDER PORTALS (clinician + administrator)
  Clara-Provider-SignIn ........ provider sign in
  Clara-Doctor-Dashboard ....... doctor dashboard (interactive)
  Clara-Doctor-Patient ......... single-patient outcome record
  Clara-Admin-Dashboard ........ administrator portal
  Clara-Admin-Providers ........ providers & permissions (Doctor / Pharmacist / Staff matrix)

All links are relative and verified: 45 pages crawl with ZERO broken
references. Images capped at 1400px (heroes are intentional 1600px JPGs);
videos transcoded to web size.

================================================================
HOW REVIEWERS NAVIGATE (no hub page — natural sign-in flow)
================================================================
PATIENT
  - Logged out: open the site root (landing page). Nav shows "Sign in".
  - Sign in (Clara-SignIn) -> lands in the patient Dashboard.

PROVIDER
  - On the patient Sign-in page there is a small "Provider sign in"
    link in the footer -> opens Clara-Provider-SignIn.
  - The provider sign-in AUTO-DETECTS the role from the email:
       * an email containing "admin"  -> Administrator portal
       * any other email              -> Doctor dashboard
  - From either dashboard, click any patient to open the full
    single-patient record.

NOTE ON ROLES: Doctor and Administrator portals are fully built.
Pharmacist and Staff are defined in the Admin > Providers & permissions
matrix and in the sign-in role list, but they do not yet have their own
separate dashboards (a view-only Staff dashboard is a planned next build,
per the Master Context). Everything else is live in this bundle.

================================================================
HOW TO PUSH IT LIVE  (GitHub Desktop — matches "clara - How We Deploy")
================================================================
The live site lives in the dashboard/ subfolder of the repo, and a tiny
root index.html redirect forwards the short link to the homepage.

1. In Finder, open this "Deploy (full site)" folder and select ALL of its
   CONTENTS (index.html, every Clara-*.html, and the asset folders).
2. Copy them INTO your repo's dashboard folder:
       Documents/GitHub/clara-wireframe/dashboard/
   Replace files when prompted. Drop the files INTO dashboard/ —
   do NOT nest a new folder (avoid dashboard/dashboard/).
3. Do NOT touch the repo ROOT index.html redirect. Leave it alone.
4. GitHub Desktop -> review changes -> Commit to main -> Push origin.
5. Wait ~1 minute, then open the link below and hard-refresh (Cmd+Shift+R).

The web uploader fails on large multi-file commits — always use GitHub Desktop.

================================================================
YOUR SHAREABLE LINK
================================================================
   https://collinnguyen123.github.io/clara-wireframe/
   (root redirect -> homepage)

   Direct homepage:  .../clara-wireframe/dashboard/Clara-Homepage-MOCK-v1.html
   Patient dashboard: .../clara-wireframe/dashboard/Clara-Dashboard-MOCK-v1.html
   Provider sign-in:  .../clara-wireframe/dashboard/Clara-Provider-SignIn-MOCK-v1.html

================================================================
WHAT CHANGED SINCE THE LAST DEPLOY (was June 21, Session 31)
================================================================
+ NEW public condition front pages: Back Pain, Nerve Pain (Session 33)
+ Sitewide copy + typography refinement, 18px body, legally-defensible
  metric wording (Sessions 33-34)
+ ENTIRE provider/clinician/administrator suite (Sessions 35-36):
  provider sign-in, doctor dashboard, single-patient record, admin
  portal, providers & permissions page, 3 provider portraits
+ Added a discreet "Provider sign in" link on the patient sign-in page
+ Removed unused leftovers (apply-clara-cream-video 2, stray .mov/.pptx/.pdf/.md)
+ All pages refreshed to their latest working versions
