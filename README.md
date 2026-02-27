# Arc — Pickleball Vision Coach

Real-time body tracking and biomechanics coaching for pickleball. 
Uses TensorFlow.js MoveNet for on-device pose estimation at 30+ FPS.

## Deploy in 60 seconds

### Option A: Vercel (Recommended)

1. Go to [vercel.com/new](https://vercel.com/new)
2. Import this folder (or push to GitHub first, then import the repo)
3. Click Deploy — done

Or from the command line:
```bash
npx vercel --prod
```

### Option B: Netlify

1. Go to [app.netlify.com/drop](https://app.netlify.com/drop)
2. Drag and drop the `public` folder
3. Done — you'll get a live URL instantly

### Option C: GitHub Pages

1. Push this repo to GitHub
2. Settings → Pages → Source: Deploy from branch → main → /public
3. Your app will be live at `username.github.io/repo-name`

**Important:** The app requires HTTPS for camera access. All three options above provide HTTPS automatically.

## How it works

- Opens your phone's camera via WebRTC
- Loads MoveNet Thunder (TensorFlow.js) for pose estimation
- Tracks 17 body keypoints at 30+ FPS
- Computes pickleball-specific biomechanics in real-time:
  - Knee bend angle (ready position)
  - Paddle hand height
  - Stance width
  - Elbow angle
  - Weight distribution
- Renders color-coded skeleton overlay
- Delivers real-time coaching tips
- Generates post-session analytics

## Tech Stack

- Pure HTML/CSS/JS (no build step)
- TensorFlow.js 4.17
- MoveNet Thunder (pose estimation)
- PWA-ready (installable to home screen)

## Requirements

- Modern browser with WebGL support
- Camera access (HTTPS required)
- Works on iPhone, Android, laptop/desktop
