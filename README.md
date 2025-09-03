# AR Birthday Surprise - Starter Project

This starter contains a web-based AR experience (mind-ar.js + A-Frame) that:
- Opens in the mobile browser (no install needed).
- Uses an **image marker** to trigger AR content.
- Shows **video** (wish.mp4) and **3D models** (cake.glb, balloons.glb).
- Works best on modern mobile browsers (Chrome on Android, Safari on iOS).

## What's included
- `index.html` - main page
- `assets/marker.jpg` - placeholder marker image (replace with your photo)
- `assets/marker.mind` - *NOT included* - you must generate this (see steps)
- `assets/cake.glb` - placeholder file (replace with a real .glb model)
- `assets/balloons.glb` - placeholder file (replace with a real .glb model)
- `assets/wish.mp4` - placeholder video (replace with your recorded message)
- `assets/song.mp3` - optional background music (you can add)

> NOTE: `.mind` file is required for mind-ar image tracking — generate it for your chosen `marker.jpg`.

## Quick Setup

1. **Pick your marker image**
   - Choose a photo or design you want to use as the trigger (e.g., a printed photo of you both).
   - Save it as `assets/marker.jpg`.

2. **Generate the `.mind` file**
   - Open: https://hiukim.github.io/mind-ar-js-doc/tools/compile
   - Upload `marker.jpg` → it will produce `marker.mind`.
   - Download and save the output as `assets/marker.mind`.

3. **Add your video and models**
   - Place your `wish.mp4` into `assets/` (replace the placeholder).
   - Place your `cake.glb` and `balloons.glb` (free models from Sketchfab or Poly Pizza).
   - Optionally add `song.mp3`.

4. **Edit greeting**
   - Open `index.html` and replace `Happy Birthday [HER_NAME] 💕` with her name.

5. **Test locally**
   - You can serve the folder with a simple local server (recommended).
     - Python 3: `python -m http.server 8000`
     - Visit on your phone: `http://<your-computer-ip>:8000/`

6. **Deploy**
   - Push to GitHub and enable GitHub Pages, OR deploy to Netlify/Vercel.
   - Copy your live URL (e.g., `https://yourusername.github.io/ar-birthday/`).

7. **QR Code**
   - Use any QR generator (e.g., https://www.qr-code-generator.com/) and paste the live URL.
   - Print the QR on the card.

## Helpful links (free assets)
- 3D models: https://sketchfab.com (filter for downloadable GLB)
- MindAR docs & marker tool: https://hiukim.github.io/mind-ar-js-doc/
- Example models & converters: https://poly.pizza

## Troubleshooting
- iOS may require a user interaction to play video. Use the "Start AR" button to allow video playback.
- If the marker is not detected, try printing the marker larger, ensure good lighting, and use a high-contrast image.

---

If you want, I can:
- Add links to specific free cake/balloon models you can download.
- Create a short example `wish.mp4` or convert a sample video (if you provide one).
- Deploy the starter repo to a temporary URL for testing.

Enjoy — and tell me if you want the repo personalized (e.g., greeting updated to "Ananya")!
