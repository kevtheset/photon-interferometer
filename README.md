# Photon Interferometer Applet

Copyright Kevin Setter.

Standalone export of the current Photon Wavepacket Lab, prepared October 16, 2026. Includes the latest label positioning, glass refraction, probability-scaled wavepackets, laser intensity controls, phase control, detector tallies, and optional nonabsorbing which-path detector.

## Files and dependencies

- `index.html`: complete editable source and ready-to-deploy application. HTML, CSS and JavaScript are embedded in this one file.
- `.nojekyll`: GitHub Pages configuration marker that bypasses Jekyll processing and serves the static files directly.
- `README.md`: setup, deployment and maintenance instructions.

There are **no external libraries, package dependencies, downloaded fonts, image assets, API keys, server requirements or build steps**. No npm install, package.json, bundler or custom Actions workflow is necessary. A modern browser is the only runtime requirement. The background-paper hyperlink is optional reading; it is not needed to run the applet.

## Try it locally

Extract the ZIP, then double-click `index.html` to open it in your browser. It works offline. Click **Send one photon** or **Start laser**. For a clear which-path comparison, select phase **0°**, observe PM1-only detection, then enable **Which-path detector** and observe the two outputs approach equal counts.

Counters reset on refresh, experiment reset, phase change or detector-mode change. Detector-mode changes also clear packets in flight.

## Deploy on GitHub Pages using the website

**Extract the ZIP first. Upload the files inside it, not the ZIP itself and not a containing folder. GitHub does not unpack an uploaded ZIP into a website.**

1. Sign in to GitHub and create a repository, for example `photon-interferometer`. A public repository works with GitHub Free. Select the option to add a README so the repository has a `main` branch.
2. Open the repository's **Code** tab and choose **Add file → Upload files**.
3. Upload the extracted `index.html`, `.nojekyll` and `README.md` into the repository root. Replace the initial README with this one if prompted. Commit the changes to `main`.
4. Confirm that `index.html` is visible immediately on the Code tab, not inside an extra folder.
5. Open **Settings → Pages**.
6. Under **Build and deployment**, set **Source** to **Deploy from a branch**.
7. Choose branch **main** and folder **/(root)**, then click **Save**.
8. Wait for the Pages deployment to finish. The Pages settings screen provides the published URL, typically `https://YOUR-USERNAME.github.io/photon-interferometer/`. If necessary, inspect the Pages run in the **Actions** tab for progress or errors.

The GitHub Pages copy will be a public website. It runs independently of ChatGPT, does not require a ChatGPT login, and does not inherit sharing restrictions from the existing hosted applet. This export does not change the existing hosted applet or automatically deploy to GitHub.

### If `.nojekyll` is hidden

On macOS, press Command+Shift+Period in Finder to show hidden files. Alternatively, in the repository choose **Add file → Create new file**, name it `.nojekyll`, put a single blank line in the editor and commit it to `main`. The file's presence is what matters.

## Updating your applet

Edit `index.html`, preview it locally, then upload the replacement to the repository root and commit it to `main`. GitHub Pages republishes changes automatically when configured as above. Refresh the published page after deployment completes. Later edits made in ChatGPT will not automatically update this separate GitHub repository; upload a new export when you want to synchronize them.

## Troubleshooting

- **404 or README shown instead of applet:** verify `index.html` is lowercase and at the root of the selected branch; check Settings → Pages is using `main` and `/(root)`.
- **ZIP shown as a download:** extract it on your computer and upload its contents instead.
- **Old appearance:** wait for deployment to succeed, then hard-refresh the page.
- **Pages unavailable:** check repository permissions and your GitHub plan. Free accounts support Pages from public repositories.

## Build configuration

Build command: **none**. Publish directory: **repository root**. Entry point: **index.html**. Static publishing marker: **.nojekyll**. No compiled output or dependency installation is required, because the source is already browser-ready.

The HTML was copied byte-for-byte from the current applet (source revision `8dbfd762240980affd8f08071ba313c4fe2cf7ec`). Hosting credentials, internal hosting configuration and Git history are excluded. The existing copyright notice is retained; no new software license has been added.

## GitHub documentation

- https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
- https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site
