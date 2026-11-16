# ✨ Gesture Particles

Real-time hand gesture recognition with MediaPipe that morphs 4,200 particles into shapes. *(Qo'l ishoralari → Zarralar)*

🔗 **Live demo:** https://qbaxtiyorov-lmnl.github.io/gesture-particles/

---

## 🖐️ Gestures *(Ishoralar)*

| Gesture | Description | Shape |
|:------:|-------------|-------|
| ✋ | Open palm | Particle cloud *(Zarralar buluti)* |
| ✌️ | Index + middle finger | "FOLLOW ME" text |
| ✊ | Fist | Rocket *(Raketa)* |
| ☝️ | Index finger only | Planet *(Sayyora)* |
| 👌 | Thumb + index touching | Heart *(Yurak)* |
| 👍 | Thumb up | Star *(Yulduz)* |
| 🤘 | Index + pinky | Lightning bolt *(Chaqmoq)* |
| 🤟 | Thumb + index + pinky | Galaxy *(Galaktika)* |
| 🖖 | Index + middle + ring finger | Atom |
| 🤙 | Thumb + pinky | Butterfly *(Kapalak)* |

If no hand is detected, the particles return to the cloud. The shape follows your hand and grows as you move it closer to the camera.

## 🚀 Usage *(Ishlatish)*

1. Open the live demo
2. Click **Kamerani yoqish** (Start camera) and allow camera access
3. Show your hand to the camera

> The camera works only over `https` or `localhost`. *(Kamera faqat https yoki localhost orqali ishlaydi.)*

### Run locally *(Lokal ishga tushirish)*

```bash
git clone https://github.com/mnbvx13/gesture-particles.git
cd gesture-particles
python -m http.server 8000
```

Then open `http://localhost:8000` in your browser.

## 🛠️ Tech *(Texnologiyalar)*

- **[MediaPipe Hands](https://github.com/google-ai-edge/mediapipe)** — hand tracking (21 landmarks)
- **HTML5 Canvas** — particle animation
- **Vanilla JavaScript** — single `index.html` file, no frameworks

## ✏️ Customize *(O'zgartirish)*

Edit the `GESTURES` object in `index.html` to change gesture-shape pairs. The particle count is set by the `N` variable.

## 🔒 Privacy *(Maxfiylik)*

Camera video is processed only in your browser and is never uploaded. *(Kamera tasviri hech qayerga yuborilmaydi.)*
