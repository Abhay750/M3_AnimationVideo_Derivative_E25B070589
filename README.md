# The Derivative: From Secant Lines to the Tangent Line

**Course:** Linear Algebra and Calculus (M3) — Internal Assessment  
**Student Name:** ABHAY KUMAR  
**URN No.:** E25B070589  
**Suggested GitHub Repository Name:** `M3_AnimationVideo_Derivative_E25B070589`

---

## Overview

This project is a publication-grade **1920×1080 (16:9)** mathematical animation explaining the geometric and algebraic foundation of the derivative—from average rate of change (secant line slope) to instantaneous rate of change (tangent line slope) as $h \to 0$.

Built using **HTML5 Canvas** and **KaTeX** (`Code/index.html`, interactive 60 fps web playback) locked to 6 original recorded narration audio files (`scene1.wav.mp3` – `scene6.wav.mp3`), and exported via headless Google Chrome (Playwright) + FFmpeg into `M3_Derivative_SecantToTangent.mp4` (**1920×1080 @ 30 fps**).

---

## Repository Contents

| File | Description |
| :--- | :--- |
| `M3_Derivative_SecantToTangent.mp4` | Final rendered 1920×1080 @ 30 fps MP4 video (`H.264` + `AAC` 48 kHz stereo audio, 4m 10.3s) |
| `Code/index.html` | Self-contained, well-commented animation web application (60 fps interactive player & `?export=1` deterministic capture mode) |
| `Code/vendor/katex/` | Bundled KaTeX CSS, JS, and fonts for 100% offline math rendering |
| `M3_Storyboard_Derivative.pdf` | Clean 6-scene M3 assessment storyboard PDF with scene thumbnails, timing, visual choreography, and narration cues |
| `scene1.wav.mp3` – `scene6.wav.mp3` | Original voice-over narration tracks recorded by Abhay Kumar |
| `README.md` | Project documentation, run instructions, and AI disclosure |

---

## Timeline & Scene Breakdown

| Scene | Timecode | Audio Track | Duration | Core Content |
| :--- | :--- | :--- | :--- | :--- |
| **Scene 0** | `0:00 – 0:04` | *(Silent)* | `4.00 s` | Opening title card, M3 subject, ABHAY KUMAR, URN No.: E25B070589 |
| **Scene 1** | `0:04 – 0:35` | `scene1.wav.mp3` | `31.35 s` | Hook: 100 m / 10 s car track, frozen speedometer `0/0 = ?` paradox, "The Derivative" reveal |
| **Scene 2** | `0:35 – 1:20` | `scene2.wav.mp3` | `44.40 s` | Formal limit definition $f'(a)=\lim_{h\to 0}\frac{f(a+h)-f(a)}{h}$, sequential symbol highlights & Learning Objective |
| **Scene 3** | `1:20 – 2:15` | `scene3.wav.mp3` | `54.85 s` | Visual intuition on $f(x)=x^2$: $P(1,1)$, $Q(1+h,(1+h)^2)$, $h \in \{2, 1, 0.5, 0.1, 0.01\} \to 0$, tangent lock |
| **Scene 4** | `2:15 – 3:16` | `scene4.wav.mp3` | `61.06 s` | Split-screen zoomed curve + 5-step KaTeX algebraic proof of $f'(1)=2$ + numerical verification table |
| **Scene 5** | `3:16 – 3:50` | `scene5.wav.mp3` | `34.06 s` | Interpretation: $y=2x-1$ rise/run step, sliding $a \to 2, 2.5$ with $f'(a)=2a$, synced speedometer gauge |
| **Scene 6** | `3:50 – 4:10` | `scene6.wav.mp3` | `20.59 s` | 3 Key Takeaways, credits, and AI disclosure |

---

## How to Run the Interactive Animation Locally

1. Start a local static server from the workspace root (recommended so browser audio policies work cleanly):
   ```bash
   python3 -m http.server 8000
   ```
2. Open [http://localhost:8000/Code/index.html](http://localhost:8000/Code/index.html) in Google Chrome, Safari, or Firefox.
3. Use the bottom player controls to **Play / Pause**, scrub the timeline, or jump directly to any scene (`S0`–`S6`).
4. Pass `?export=1` in the URL (`Code/index.html?export=1`) to hide all player UI chrome for clean 1920×1080 headless capture via `window.renderAtTime(seconds)`.

---

## AI Disclosure

- **Original Narration & Concept Ownership:** Recorded voice-over audio (`scene1.wav.mp3` – `scene6.wav.mp3`) and mathematical exposition by **ABHAY KUMAR** (**URN No.: E25B070589**).
- **AI Assistance:** **Gemini** and **Antigravity** assisted with storyboard formatting, HTML5 Canvas / KaTeX animation code, audio-timestamp synchronization, and FFmpeg video export pipeline.
