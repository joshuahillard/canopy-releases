# Canopy releases

Built desktop apps for Canopy on Windows and macOS. The source code lives in a private repo; this repo only holds the release files.

## Install

- Windows: download `Canopy_<version>_x64-setup.exe` from the latest release and run it.
- macOS: download `Canopy_<version>_universal.dmg` and drag Canopy to Applications. The app is not signed by Apple, so a browser download shows a warning the first time; allow it in System Settings > Privacy & Security > Open Anyway. A Terminal download skips the warning:

```
cd ~/Downloads && curl -fLO "$(curl -fsSL https://api.github.com/repos/joshuahillard/canopy-releases/releases/latest | grep -o 'https://[^"]*universal\.dmg' | head -1)" && open Canopy_*_universal.dmg
```

After the first install, Canopy updates itself from this repo.
