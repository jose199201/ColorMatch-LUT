# ColorMatch LUT

**→ [Open the app](https://jose199201.github.io/ColorMatch-LUT/)**

Browser-based color grading tool. Upload a source image and a color reference, and the app automatically transfers the color palette. No install, no server — everything runs locally in your browser.

---

## What it does

- Analyzes the color distribution (mean + standard deviation per RGB channel) of both images
- Transfers the reference palette to the source image using the Reinhard method with soft-clamp to preserve highlights
- Lets you fine-tune strength, brightness, contrast, and saturation in real time
- Exports a **33×33×33 3D LUT in `.cube` format** compatible with Photoshop, Lightroom, DaVinci Resolve, and Premiere Pro
- Shows comparative histograms and per-channel color delta

## How to use the LUT in Photoshop

1. Export the `.cube` from the app
2. `Layer → New Adjustment Layer → Color Lookup`
3. In the properties panel: `Load 3D LUT...` → select your `.cube` file

## Supported formats

Input: JPG · PNG · WebP  
LUT export: `.cube` (standard 3D LUT)  
Image export: PNG

## Privacy

No image ever leaves your browser. No backend, no server, no tracking.

---

Made with vanilla HTML + Canvas API
