# 🎧 Modular Focus Music App - FocusTune

Welcome to the **Modular Focus Music App** – a dynamic sound-layering experience designed to help users enhance concentration and flow by customizing their own focus music in real time.

This app allows users to toggle individual instruments, adjust their volume, apply effects like reverb or filters, and mix them into a seamless ambient soundtrack. Think of it as a real-time, minimal DAW for productivity.

---

## 🚀 Project Goals

- Allow users to build **custom ambient focus music** from layered instrument loops.
- Use **looped .wav/.ogg stems**, not MP3 playback.
- Provide **real-time audio control** over each instrument (volume, enable/disable, effects).
- Target web and mobile platforms.
- Prioritize **low latency**, **zero-gap looping**, and **smooth transitions**.

---

## 🛠️ Tech Stack

| Layer      | Tools / Frameworks                             |
|------------|------------------------------------------------|
| Frontend   | React.js or Flutter (TBD)                      |
| Audio      | WebAudio API / Tone.js / AudioKit / Oboe SDK   |
| Cross-Platform | React Native (or Flutter for native audio support) |
| Backend (Optional) | Firebase / Supabase (for user presets and metadata) |

---

## 🧱 Core Features

- 🎚 **Instrument Mixer**: Toggle and control multiple instrument layers.
- 🔁 **Perfect Loop Syncing**: All loops align in time signature (e.g., 120 BPM, 4 bars).
- 🎧 **Effect Chains**: Optional reverb, filters, delay per channel.
- 🧠 **Presets**: Predefined mixes like "Deep Focus", "Morning Flow", "Creative Energy".
- 📅 **Session Scheduler**: Optional Pomodoro or deep-work timers tied to music state.

---

## 🎵 Audio Asset Strategy

- Use **looped WAV/OGG files**, trimmed to match time signature grid.
- All loops must follow a master tempo (e.g., 120 BPM, 4/4).
- Each loop is an **isolated instrument**: e.g., pad, piano, lo-fi drum, white noise, etc.
- Loops must start at sample-perfect alignment to avoid drift.

Example structure:
/assets/audio/
└── pad_loop.wav
└── pluck_loop.wav
└── rain_fx_loop.wav
└── sub_bass_loop.wav

yaml
Copy
Edit

---

## 🧠 Codex Instructions (For AI Assistance)

If you're using GitHub Copilot or ChatGPT Codex to assist with development, here’s how to prompt effectively:

"You are building a modular ambient music app. Each instrument is a looped audio buffer (WAV/OGG).
Loops must be in perfect sync. User should be able to toggle each instrument on/off, change volume, and apply optional filters.
Use Tone.js or WebAudio API. UI should be React-based with sliders and toggle buttons per track."

yaml
Copy
Edit

---

## 📁 Project Structure (Planned)

/src/
└── components/
└── MixerChannel.jsx
└── MasterControls.jsx
└── AudioEngine.js
└── assets/
└── audio/
└── App.jsx
└── index.html
└── styles/
└── main.css

yaml
Copy
Edit

---

## 🔮 Future Enhancements

- AI-based “Mood Mixer” that adjusts instruments based on user input or time of day.
- Binaural beats generation.
- Offline PWA support.
- Open marketplace for custom instrument loops.

---

## 🧑‍💻 Contributing

We welcome builders, audio engineers, and designers!
Please follow our [contributing guide](CONTRIBUTING.md) (TBD) and feel free to submit ideas via GitHub Issues.

---

## ⚖️ License

MIT License. All included audio files are either royalty-free or open-source under Creative Commons licenses. See `/assets/audio/LICENSE.md` for details.

---

## ❤️ Inspiration

This app is inspired by a desire to give users control over their productivity environment—without ads, interruptions, or overproduced audio. Pure sound. Pure focus. Pure you.

---

> “Music is the space between the notes.” – Claude Debussy  
