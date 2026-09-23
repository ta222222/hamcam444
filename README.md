# hammercam 4.0

Offline Floyd–Steinberg dither camera with iPhone-style photo & video capture.

## Open

Serve the folder over HTTPS or localhost (required for camera + offline install):

```bash
cd ~/Desktop/hammercam-4.0
python3 -m http.server 8080
```

Then on your phone (same Wi‑Fi): `https` tunnel, or open `http://YOUR_MAC_IP:8080`.

For camera + “Add to Home Screen” offline use, prefer HTTPS (e.g. Cloudflare tunnel / ngrok).

## Use

1. **Start camera**
2. **Photo** mode — tap the shutter → share sheet → **Save Image** (Photos)
3. **Video** mode — tap shutter to start/stop, or hold shutter in Photo mode to record → **Save Video**
4. Zoom bar is digital (0.5 / 1× / 2× / 4× / 6×)
5. After first load, the service worker caches the app for **offline** use

## Notes

Browsers cannot write silently into the Photos library. Saving uses the system share sheet (same pattern as other iOS camera web apps). Add to Home Screen for a fullscreen offline app icon.
