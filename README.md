# FaceFrame Lab

A responsive, browser-based facial landmark and proportion explorer. Uses MediaPipe Face Landmarker in the browser to estimate a few 2D geometric properties from an uploaded photo or webcam capture.

## Features
- Webcam access and capture in-browser
- Upload image input
- Face landmark overlay
- Approximate landmark symmetry, vertical thirds balance, eye-spacing ratio, and face height/width ratio
- Responsive dark interface
- No photo uploads, backend, account, or database
- Vercel-ready static deployment

## Run locally
Serve this folder over localhost (camera APIs require HTTPS or localhost). For example:

```bash
npx serve .
```

Open the local URL and allow camera access, or upload an image. The app loads MediaPipe assets from public CDNs, so internet access is required for model loading.

## Deploy to Vercel
Import this repository into Vercel. No build command is needed; the root directory contains `index.html`. `vercel.json` supplies clean static routing and security headers.

## Responsible use
The displayed geometry index is **not an attractiveness score** and is not validated for clinical, scientific, casting, hiring, or model-industry decisions. Facial aesthetics are subjective and culturally variable. Image angle, lighting, expression, and camera distortion affect measurements. No face image is sent to an application server by this code; browser requests fetch the public model files only.

## License
MIT
