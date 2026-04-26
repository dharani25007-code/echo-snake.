<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:08090d,50:4c1d95,100:08090d&height=200&section=header&text=ECHO%20SNAKE&fontSize=52&fontColor=a78bfa&fontAlignY=40&desc=Your%20Past%20Hunts%20You&descAlignY=60&descSize=18&descColor=6366f1&animation=fadeIn"/>
</div>

<div align="center">

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Canvas API](https://img.shields.io/badge/Canvas_API-Vanilla-a78bfa?style=for-the-badge)
![No Dependencies](https://img.shields.io/badge/Dependencies-Zero-4ecdc4?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

> 🐍 Classic Snake — but your ghost follows your exact path with a **5-second delay.**
> Survive long enough and your past becomes your deadliest enemy.

**[▶ Play Now](#getting-started)** · **[View Source](echo_snake_game.html)**

</div>

---

## 🎮 What Makes It Different

Normal Snake: avoid walls, avoid yourself.

**Echo Snake:** after 5 seconds, a **ghost snake** spawns and replays your exact movement history. It follows every turn you made — perfectly. The longer you survive, the closer your echo gets.

> *"You're not just playing against the game. You're playing against yourself."*

---

## ✨ Features

| Feature | Detail |
|---|---|
| 👻 **Echo Ghost** | Your past path replays as a red ghost snake after 5 seconds |
| 📊 **Echo Bar** | Live progress bar shows exactly when your echo activates |
| ⚡ **Level System** | Speed increases as your snake grows |
| ✨ **Particles** | Gold burst particles on every apple collected |
| 🎮 **3 Control Modes** | Keyboard (Arrow / WASD) · Touch swipe · On-screen D-pad |
| 📱 **Mobile Ready** | Touch controls + swipe support on canvas |
| 🏆 **Best Score** | Persists across rounds during the session |
| 🎨 **Dark Theme** | Deep purple + indigo aesthetic with pixel font |

---

## 🕹️ How to Play

1. **Move** your purple snake to eat the yellow apple
2. Watch the **Echo Bar** — when it fills, your ghost activates
3. The **red ghost** replays your exact movements from 5 seconds ago
4. **Don't collide** with walls, yourself, or your echo
5. Survive as long as possible — your echo gets longer as you do

### Controls

| Input | Action |
|---|---|
| `Arrow Keys` / `WASD` | Move snake |
| Swipe on canvas | Move snake (mobile) |
| D-pad buttons | Move snake (touch) |

---

## 🚀 Getting Started

Zero setup. No install. No server needed.

```bash
git clone https://github.com/dharani25007-code/echo-snake.git
cd echo-snake
# Just open the file in your browser:
open echo_snake_game.html
```

Or drag the `.html` file into any browser — it works instantly.

---

## 🏗️ Technical Details

Built with **zero dependencies** — pure HTML5 Canvas and vanilla JavaScript.

| Component | Implementation |
|---|---|
| Rendering | HTML5 `<canvas>` with `roundRect`, alpha layering |
| Echo System | Circular history buffer — replays head positions with `ECHO_FRAMES` delay |
| Ghost Logic | Tail slice of history array, reversed — mirrors exact player path |
| Particles | 6-particle burst per apple, velocity + lifetime system |
| Speed Scaling | `max(80, 200 - (level-1) * 18)` ms per frame |
| Mobile Input | `touchstart` / `touchend` delta with `e.preventDefault()` |
| Font | Press Start 2P (Google Fonts) — retro pixel style |

---

## 🎨 Color Palette

| Element | Color |
|---|---|
| Background | `#08090d` |
| Canvas | `#0d0f1a` |
| Player Snake (head) | `#a78bfa` (purple) |
| Player Snake (body) | `#4c1d95` (deep purple) |
| Echo Ghost | `#f87171` (red) |
| Apple | `#fbbf24` (gold) |
| Accent / UI | `#6366f1` (indigo) |

---

## 📄 License

MIT License — see [LICENSE](LICENSE)

---

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:4c1d95,100:08090d&height=120&section=footer&text=Don't%20let%20your%20past%20catch%20you.&fontSize=14&fontColor=a78bfa&fontAlignY=65&animation=fadeIn"/>

**Built by [Dharanidharan M](https://github.com/dharani25007-code) · Coimbatore, India 🇮🇳**
</div>
