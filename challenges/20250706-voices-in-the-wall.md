# 🎯 Patch Challenge: **Voices in the Wall**

## 🌑 Theme
You are sculpting a wall of sound built from **ghosts of real places** and **metallic echoes**. The result should feel like half-understood speech and flickering signal fragments trapped in a structure that’s alive with voltage and distortion.

The soundscape should be reactive, textural, and **never fully intelligible**, but **evocative** — like listening through concrete.

---

## 🎧 Sound Sources

### **Morphagene**
- Load a reel from your field recording (street festival ambience)
- Add **splice points every ~300ms to 1s** — capturing single syllables, room tone, or brief background events
- Select a **slice loop** with ambiguous vocal content or texture
- Set **Gene Size** small — modulate it with slow, unstable CV
- Use **Organize** to scan across adjacent slices slowly
- Optionally modulate **Slide** for glitch or shifting phrasing
- Use **EOSG** to clock Chaos for variable-rate gate rhythm

### **Incus Iteritas Alia (IIA)**
- Set up short, unpredictable FM-rich bursts or glitch tones
- Use CV to modulate:
  - **Weight** — harmonic density
  - **Alloy** — algorithm selection/metallic quality
  - **Shape** — waveform skew
  - **Temper** — brightness or noise content
  - **Attack** and **Time** — control voice envelope shape
- Trigger with looping gates from Chaos or Morphagene EOSG
- Adjust parameters so that IIA cuts in and out like a corrupted response voice
- Optionally post-process with **Sealegs** for spatial smear or warble

---

## 🧩 Modulation & Structure

| Source                  | Destination                    | Notes |
|-------------------------|--------------------------------|-------|
| **Chaos**               | Organize, IIA parameters, gate | Use looping CVs on 2–3 channels, some synced, some not |
| **IIA envelope out**    | Sealegs or Bib CV inputs       | Shape FX dynamics based on tone presence |
| **Sealegs Aux (env follower)** | Chaos transpose or Bib mix | Drive structure from output intensity |
| **Atte**                | CV shaping (offset/invert)     | Adjust CV ranges for nuance |
| **EOSG (from Morphagene)** | Chaos clock input            | Create timing that reflects reel structure |

---

## 🌀 FX Routing

- **Morphagene → Bib → Mixer**
- **IIA → Sealegs → Mixer**
  - Modulate delay feedback and modulation rate
  - Clock Sealegs *if desired* — or leave free-running for drift

---

## 🎛️ Performance Interaction Suggestions

- Manually modulate **Gene Size** or **Varispeed** du
