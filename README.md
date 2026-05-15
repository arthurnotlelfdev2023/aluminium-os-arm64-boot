# 🔥 Aluminium OS ARM64 Boot via GitHub Actions

Run the leaked Aluminium OS `.img` on a **free GitHub ARM64 runner** and access it from your browser!

## How To Use

### Step 1 — Add your ngrok token
1. Sign up free at [ngrok.com](https://ngrok.com)
2. Copy your authtoken from the dashboard
3. Go to your repo → **Settings → Secrets and Variables → Actions**
4. Add a new secret named `NGROK_TOKEN` and paste your token

### Step 2 — Upload your .img file
Upload your `aluminium-os.img` somewhere with a direct download link:
- Google Drive (use a direct link generator)
- Dropbox (change `dl=0` to `dl=1`)
- Any file host with a direct `.img` URL

### Step 3 — Run the workflow
1. Go to **Actions** tab in this repo
2. Click **Boot Aluminium OS ARM64**
3. Click **Run workflow**
4. Paste your `.img` direct download URL
5. Hit **Run workflow** and wait ~2 minutes

### Step 4 — Open in browser
Watch the Action logs — it will print a URL like:
```
https://xxxx-xx-xx-xx-xx.ngrok-free.app
```
Open that in your browser. You'll see noVNC — click **Connect** and you're IN! 🎉

## Notes
- The runner is a real ARM64 machine — no emulation lag! 🚀
- Session lasts up to **6 hours** (GitHub Actions limit)
- ngrok free tier URL changes every run
- You need a free ngrok account for the tunnel
