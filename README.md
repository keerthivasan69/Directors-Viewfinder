# Director's Viewfinder — browser proof of concept v0.1

Open `index.html` from an HTTPS host or from localhost. For local testing:

```bash
python3 -m http.server 8000
```

Then visit http://localhost:8000/ on the same computer. For a phone, deploy to HTTPS (for example GitHub Pages, Netlify, or Vercel). Merely opening the file directly may not allow camera access.

## Features
- Live browser camera preview, camera-source selection
- Illustrative cinema camera/sensor presets, custom sensor dimensions
- Spherical and anamorphic FOV estimation
- Focal-length and aspect-ratio controls
- Coverage warning for unsupported fields of view
- Save a cropped PNG reference

## Limitations
This is **not** a production-calibrated viewfinder. Sensor presets are illustrative, source camera FOV inputs are manual, and there is no lens distortion calibration, validated device matrix, database, account, or cloud storage. The browser does not reliably expose physical camera metadata. The preview assumes a rectilinear source camera. Captured PNG files do not yet embed metadata. Frame comparison needs real-world optical validation.
