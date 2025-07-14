# 🎯 Patch Challenge: **Flesh + Circuits v2**

## 🧠 Theme
The machine wakes, remembers, and mutates. You’ll use **self-patching**, **chaos-driven modulation**, and **feedback-aware effects** to build a generative soundscape. The patch lives and grows in a confined world — the 3D-printed rack — with **no external clocks or modulation**.

---

## 🧰 Modules Used (3D-Printed Case Only)

| Module                         | Role                                     |
|--------------------------------|------------------------------------------|
| **Manis Iteritas Alia**        | Core voice — harsh, evolving tone        |
| **Clank Chaos**                | Aleatoric CV and gate sequencing         |
| **Bib (Crey Emporium)**        | Multi-effect: distortion, echo, reverb   |
| **Sealegs (Intellijel)**       | Stereo delay, reverb, character FX       |
| **Befaco Atte**                | Quad attenuator/inverter, CV shaping     |
| **Happy Nerding 4x Stereo Mix**| Final mix & stereo balancing             |

---

## 🎵 Patch Flow

### 1. **Voices**
- **Morphagene**: Reels provide evolving sound material  
  - Output → **Bib** → **Mixer**
  - Morphagene parameters (Gene Size, Slide, VariSpeed, etc.) modulated by Chaos + Ōchd
  - **EOSG (End of Slice)** → **Chaos Clock Input** — for variable-rate clocking

- **Manis Iteritas Alia**: Set to tame tone (knobs CCW), CV modulation drives instability  
  - Output → **Sealegs**
  - Delay Feedback and Rate modulated by Chaos or Sealegs mod out
  - Envelope out used for dynamics shaping (e.g., Sealegs feedback or Bib CV)

### 2. **Modulation**
- **Chaos**:
  - Drives pitch, CV, and gate signals for Morphagene and Manis
  - Receives variable clock from **Morphagene EOSG**

- **External LFOs (Ōchd)**:
  - Used for bipolar modulation of Morphagene’s Gene Size and VariSpeed (outside rack constraint, optional)

- **Atte**:
  - Shapes CV signals going into Morphagene and Manis
  - Used to invert/scale Sealegs Aux or Manis Envelope

---

## 🔁 FX Routing

- **Bib**: Dedicated FX path for **Morphagene**
- **Sealegs**: Dedicated FX path for **Manis**
  - Sealegs is clocked by Chaos, introducing temporal instability
  - FX paths intentionally separated to preserve sonic contrast between voices

---

## 🎧 Sound Goals

| Goal                               | Achieved? |
|------------------------------------|-----------|
| Asymmetric melodies                | Partially (slow and irregular; more random than melodic) |
| Distorted yet reactive textures    | ✅ Achieved through Bib + Chaos-modulated Manis |
| Ghostly tails                      | ✅ Achieved but carefully dialed to avoid mud |
| Reactive patch behavior            | ✅ High variability from modulation and feedback loops |

---

## 📝 Reflection

- **Clocking with EOSG** was especially interesting and promising  
  > Plan to explore more predictable modulation by using equal-length slices

- **Thematic execution** was moderate:  
  > Transitions (e.g., “Awakes → Remembers”) could be better defined via structured modulation and performative gestures

- **Hand-played modulation** was critical for expressive scene shifts  
  > Modulating Gene Size or Varispeed manually helped guide pacing and transitions

- **Learning goals met**:
  - Patch was reactive, expressive, and fun
  - Theme was served well despite being non-musical
  - Modulation routing revealed new creative feedback loops

---

## 💡 Future Improvements

- Use consistent slice lengths in Morphagene for more controlled EOSG clocking
- Add Ōchd to the 3D-printed case (fits in side 4hp space) to stay within constraint
- Consider more defined performative controls for transitions (e.g., manual gate muting or scene switches)


## Debrief

[Debrief notes](./20250703-small-case-debrief.md)