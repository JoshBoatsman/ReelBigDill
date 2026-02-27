# Arc — Pickleball Vision Coach

Real-time biomechanical coaching for pickleball using computer vision.

## Features
- **5-Rule Biomechanical Engine**: Transition panic, split step, wrist snap, backswing, non-dominant arm
- **Audio Coaching**: Real-time voice cues through Web Speech API
- **Video Replay**: Post-session playback with skeleton overlay, adjustable speed
- **Session History**: Persistent tracking across sessions with trend analysis
- **17-Point Pose Estimation**: TensorFlow.js MoveNet Thunder, 30 FPS on-device

## Deploy

### Vercel (recommended)
1. Push this folder to a GitHub repo
2. Go to vercel.com/new → Import → Deploy
3. HTTPS is automatic (required for camera)

### Netlify
1. Drag the `public` folder to app.netlify.com/drop
2. Done — live in 60 seconds

### GitHub Pages
1. Push to GitHub, enable Pages from Settings → Pages → main branch → /public
2. HTTPS automatic on github.io domains

## Tech Stack
- TensorFlow.js 4.17 + MoveNet Thunder (single-pose)
- Web Speech API for audio coaching
- MediaRecorder API for video capture
- LocalStorage for session persistence
- Zero backend, zero dependencies, fully on-device
