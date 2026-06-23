<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:08090d,50:4c1d95,100:08090d&height=200&section=header&text=ECHO%20SNAKE&fontSize=52&fontColor=a78bfa&fontAlignY=40&desc=Your%20Past%20Hunts%20You&descAlignY=60&descSize=18&descColor=6366f1&animation=fadeIn"/>

  
</div>

<div align="center">
  
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![No Dependencies](https://img.shields.io/badge/Dependencies-Zero-4ecdc4?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)
![Version](https://img.shields.io/badge/Version-2.0-a78bfa?style=for-the-badge)

> 🐍 Classic Snake — but your ghost follows your exact path with a **5-second delay.**
> Survive long enough and your past becomes your deadliest enemy.

**[▶ Play Now](https://dharani25007-code.github.io/echo-snake./)** · **[View Source]()**

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
| 👻 **Echo Ghost** | Your past path replays as a ghost snake after 5 seconds — perfectly mirroring every move |
| 🔥 **Combo System** | Chain apple pickups quickly to build a multiplier up to **×8** |
| ⚡ **Power-Ups** | 4 types spawn randomly — Speed Boost, Ghost Shield, Score Doubler, Slow Echo |
| 🎨 **5 Color Themes** | Switch between Void, Neon, Matrix, Amber, and Ice — live, even mid-game |
| 📊 **Echo Bar** | Live progress bar shows exactly when your echo activates — turns red at 80% |
| 🏆 **Level System** | Speed scales as your snake grows — max challenge at high levels |
| ✨ **Particles & Floats** | Burst particles + floating score text on every apple eaten |
| 💥 **Screen Shake** | Impact shake on death for tactile feedback |
| 🛡️ **Shield Ring** | Visual ring pulses around your head when Ghost Shield is active |
| 🎮 **3 Control Modes** | Keyboard (Arrow / WASD) · Touch swipe on canvas · On-screen D-pad |
| 📱 **Mobile Ready** | Fully playable on touch devices |
| 🏅 **Best Score** | Persists across rounds within the session |

---

## ⚡ Power-Ups

Four power-up types randomly appear on the board. Grab them before they expire!

| Icon | Power-Up | Effect |
|------|----------|--------|
| ⚡ | **Speed Boost** | Moves faster temporarily — great for escaping tight spots |
| ✦ | **Ghost Shield** | Protects from one echo collision — shows a glowing ring around your head |
| ×2 | **Score Doubler** | All points doubled for the duration |
| ● | **Slow Echo** | Delays when the echo activates — buys you more breathing room |

---

## 🔥 Combo System

Eat apples in rapid succession to multiply your score:

```
x1  →  x2  →  x3  →  ... →  x8 (MAX)
```

- Combo resets if you wait too long between pickups
- Higher combos turn the HUD **gold → pink**
- Pair with the ×2 power-up for massive score bursts

---

## 🕹️ How to Play

1. **Move** your snake to eat the pulsing apple
2. Watch the **Echo Bar** — when it fills, your ghost activates
3. The **ghost** replays your exact movements from 5 seconds ago
4. **Chain apples** fast to build your combo multiplier
5. **Grab power-ups** before they disappear from the board
6. **Don't collide** with walls, yourself, or your echo

### Controls

| Input | Action |
|---|---|
| `Arrow Keys` / `WASD` | Move snake |
| Swipe on canvas | Move (mobile) |
| D-pad buttons | Move (touch UI) |
| Theme dots | Switch color theme |

---

## 🎨 Color Themes

| Theme | Snake | Echo | Apple | Vibe |
|-------|-------|------|-------|------|
| **Void** | `#a78bfa` purple | `#f87171` red | `#fbbf24` gold | Default dark magic |
| **Neon** | `#f472b6` pink | `#fb923c` orange | `#a3e635` lime | Arcade night |
| **Matrix** | `#34d399` green | `#f43f5e` rose | `#facc15` yellow | Digital rain |
| **Amber** | `#f59e0b` amber | `#818cf8` indigo | `#f472b6` pink | Warm glow |
| **Ice** | `#60a5fa` blue | `#fb7185` coral | `#a78bfa` violet | Cryo chill |

---

## 🚀 Getting Started

Zero setup. No install. No server needed.

```bash
git clone https://github.com/dharani25007-code/echo-snake.git
cd echo-snake
# Open in any browser:
open echo_snake_game.html
```

Or just drag the `.html` file into any browser — it works instantly.

---

## 🏗️ Technical Details

Built with **zero dependencies** — pure HTML5 Canvas and vanilla JavaScript.

| Component | Implementation |
|---|---|
| Rendering | HTML5 `<canvas>` with `roundRect`, alpha layering, shadow blur |
| Echo System | Circular history buffer — replays head positions with `ECHO_FRAMES` delay |
| Ghost Logic | Tail slice of history array, reversed — mirrors exact player path |
| Combo Engine | Frame-delta tracking — resets combo if gap exceeds `comboWindow` frames |
| Power-Up System | Probabilistic spawn, per-item lifetime timer, effect flag state |
| Particles | Velocity + gravity + lifetime system, per-apple burst |
| Float Text | Y-drift labels with fade-out — score feedback above eaten apple |
| Screen Shake | Exponential decay on X/Y offset applied at draw time |
| Themes | Runtime swap of color palette object — all draws reference `T()` |
| Speed Scaling | `max(90, 200 - (level-1) * 15)` ms — modified by Speed Boost power-up |
| Mobile Input | `touchstart` / `touchend` delta swipe with `e.preventDefault()` |
| Font | Press Start 2P (Google Fonts) — retro pixel style |

---

## 📄 License

MIT License — see [LICENSE](LICENSE)

---

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:4c1d95,100:08090d&height=120&section=footer&text=Don't%20let%20your%20past%20catch%20you.&fontSize=14&fontColor=a78bfa&fontAlignY=65&animation=fadeIn"/>

**Built by [Dharanidharan M](https://github.com/dharani25007-code)**

</div>
