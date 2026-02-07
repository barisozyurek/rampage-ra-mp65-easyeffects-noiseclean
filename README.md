# 🎤 Rampage RA-MP65 — EasyEffects NoiseClean Preset

> **Main language: English**  
> Türkçe sürüm için: [README_TR.md](README_TR.md)

This repository provides a carefully tuned **EasyEffects preset** for the  
**Rampage RA-MP65 X-FUSE USB microphone** on Linux (PipeWire).

The goal of this preset is to **eliminate constant background noise** such as:

- Electronic hiss
- High-frequency “bip” tones
- USB ground noise
- Low-level static hum

Unlike simple noise gate solutions, this preset uses **two neural-network based
noise suppression engines: RNNoise and DeepFilterNet.**  
These models analyze the signal and suppress only the noise while preserving
the voice.

It is designed for:

- 🎮 Gaming & Discord
- 🎙 Voice chat
- 📹 Streaming & recording
- 💻 Meetings (Zoom, Teams, etc.)

---

## 📁 Files

- `rampage-ra-mp65-clean.json` — EasyEffects preset file

---

## 🧰 Requirements

- Linux with **PipeWire**
- **EasyEffects 7+**
- **DeepFilterNet** plugin

### Install DeepFilterNet (Arch / CachyOS)

```bash
paru -S libdf-git libdeep_filter_ladspa-git
```

For other distros, search your package manager for:  
`deepfilter`, `libdeep_filter`, or `ladspa-deepfilter`.

---

## ⚙ Installation

1. Open **EasyEffects**
2. Go to **Presets → Import**
3. Select `rampage-ra-mp65-clean.json`
4. Apply the preset
5. Make sure your microphone input is selected in EasyEffects

---

## 🔊 Effect Chain Explained

| Effect | Purpose |
|--------|---------|
| **RNNoise** | Removes steady broadband noise |
| **DeepFilterNet** | Neural-network based voice isolation |
| **Gate** | Mutes mic when you are silent |

---

## 🛠 Tips

- Keep your mic volume around **70–85%**
- Avoid USB hubs (connect directly to PC)
- Use a pop filter if possible
- If your voice sounds cut, slightly lower Gate threshold
