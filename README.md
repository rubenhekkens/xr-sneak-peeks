# XR Sneak Peeks

Five real-time 3D demos, each a **single self-contained HTML file** (three.js 0.160 from CDN, no build step).

**▶ Live: https://rubenhekkens.github.io/xr-sneak-peeks/**

| # | Demo | What it is |
|---|------|-----------|
| 1 | [Ghost Flow](1-gas-curtain.html) | Real-time gas-curtain contamination-control sandbox — 20,000 particles, live protection efficiency, guided demo mode |
| 2 | [Teardown](2-exploded-machine.html) | A real 14-part drill assembly (FBX + full PBR textures) exploding under HDRI lighting |
| 3 | [Silicon Dive](3-powers-of-chip.html) | Powers of Ten into a chip: motherboard → die → FinFET → silicon lattice in one scroll |
| 4 | [Terrainwave](4-terrainwave.html) | Your music carved into a synthwave mountain range — drop an MP3, beat-detected camera |
| 5 | [Holo Twin](5-machine-twin.html) | Holographic digital twin of a vacuum vessel: live telemetry, injectable anomaly |

All demos share a cinematic pipeline: ACES tone mapping, Unreal bloom, film grain, vignette and chromatic aberration.

## Models

- `assets/drill.fbx` + `assets/textures/` — 14-part drill assembly (Tripo AI, via Unity project)
- `assets/vessel.glb`, `assets/optic.glb` — generated with the [Tripo AI](https://www.tripo3d.ai) text-to-3D API
- HDRI from the three.js example assets

## Run locally

```bash
python -m http.server 8090
# open http://localhost:8090
```

(Internet required — three.js loads from jsDelivr.)

Built by Ruben Hekkens with Claude Code.
