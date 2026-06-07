CLARA DASHBOARD DEPLOY BUNDLE
=============================
Built: June 7, 2026 (Session 14)

WHAT THIS IS
A self-contained, web-optimized copy of the patient Dashboard and all
seven education pages. Only assets actually referenced by the pages are
included; images are downscaled to 1600px web size. 133 MB total.

  index.html ................ the Dashboard (also kept as Clara-Dashboard-MOCK-v1.html)
  Education Section (Knee OA Pain)/ ... all 7 education pages + images + video

HOW TO DEPLOY TO GITHUB PAGES (clara-wireframe repo)
1. Open github.com/collinnguyen123/clara-wireframe
2. Replace the contents of the dashboard/ folder with the contents of
   this folder (keep the folder structure exactly as is).
   Easiest: GitHub Desktop or git; the web uploader also accepts
   dragging the whole folder.
3. Commit. Pages redeploys automatically in about a minute.
4. Check: https://collinnguyen123.github.io/clara-wireframe/dashboard/

NOTES
- The largest single file is How-to-apply-demo.mp4 (about 20 MB),
  well under GitHub's 100 MB per file limit.
- Links between dashboard and education pages are relative, so the
  bundle works at any URL and also opens fine locally.
- Full resolution image masters remain in
  Technology/Wireframes/Education Section (Knee OA Pain)/ on the Desktop.
