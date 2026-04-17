# FlowReel (TikTok-style mock)

Static HTML mock feed intended to run on **GitHub Pages**.

## Run locally

- Open `index.html` in a browser, or serve the folder with any static server.

## Videos

- `assets/videos/meditate1.mp4` is included in the repo.
- `meditate2.mp4` is **~103MB**, which is slightly above GitHub’s **100MB** normal file limit.

### Option A (recommended): host `meditate2.mp4` as a GitHub Release asset

1. Create a Release in your repo on GitHub and upload `meditate2.mp4` as an asset.
2. Copy the asset’s direct download URL.
3. In `index.html`, replace:

`REPLACE_WITH_GITHUB_RELEASE_ASSET_URL`

with your copied URL.

The page will automatically fall back to that URL if `assets/videos/meditate2.mp4` is missing.

### Option B (local only): copy `meditate2.mp4` into the project

Copy your file to:

`assets/videos/meditate2.mp4`

It will work locally, but it won’t be committed.

## Deploy to GitHub Pages

1. Create a new GitHub repository (public).
2. Push this folder as the repository contents.
3. In GitHub: **Settings → Pages**
   - Source: **Deploy from a branch**
   - Branch: `main` (or `master`)
   - Folder: `/ (root)`

Then wait for GitHub Pages to publish and open the Pages URL.

