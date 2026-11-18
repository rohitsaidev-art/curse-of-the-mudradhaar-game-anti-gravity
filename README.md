# Curse of the Mudradhaar 👹⚡
### A Dark Fantasy Webcam Mudra Combat Game (Antigravity)

**Curse of the Mudradhaar** is a real-time first-person gesture combat game inspired by ancient Indian dark fantasy and tantrik lore. The player takes on the mantle of a **Tantrik warrior** trapped in the subterranean temple cavern of **Daanav** (a horned demon entity).

Using **Google MediaPipe Hands**, the game tracks your physical hands in real-time through your webcam. Match the prompted two-hand sacred Mudras before the countdown expires to channel divine spells, or get torn apart by the Daanav's wrath!

---

## 🎮 Gameplay & Mechanics

1. **First-Person View:** You see your crimson Tantrik hands adorned with sacred ash (*Tripundra*), rudraksha beads, red silk wrist threads, and gemstone ritual rings.
2. **Dual-Mudra Combos:** The game prompts a two-hand combination (e.g., `🤘 + 🖐`, `✊ + ✌️`, `🤘 + 👍`).
3. **Real-Time Webcam Vision:** Using Google MediaPipe, the browser tracks your physical left and right hands simultaneously at 60 FPS.
4. **Spell Casting:** If you hold the correct two-hand combo before the timer runs out:
   - A divine spell blasts the Daanav's core.
   - Searing holy fire, golden embers, and dark smoke erupt.
   - Daanav flinches in pain (*Hurt State with cracking magma veins*).
5. **Daanav Counter-Attack:** If time runs out or you fail to form the signs:
   - Daanav lunges forward roaring (*"ENOUGH!"*, *"STOP!"*, *"FOOLISH MORTAL!"*).
   - Screaming red damage vignette flashes as the player takes heavy damage.
6. **Victory / Defeat:** Vanquish the Daanav by depleting his 100 HP, or fall in battle if your Tantrik HP reaches 0.

---

## 🪬 Sacred Mudras Recognized

| Emoji | Mudra Name | Gesture Description |
| :---: | :--- | :--- |
| **🤘** | **Karana Mudra** | Index & Pinky extended, Middle & Ring curled (Rock Horns) |
| **🖐** | **Abhaya / Pataka** | Open Palm facing forward, fingers spread |
| **✊** | **Mushti Mudra** | Clenched Fist (all 4 fingers curled) |
| **✌️** | **Kartarimukha** | Index & Middle fingers extended (Peace / Victory) |
| **☝️** | **Suchi Mudra** | Index finger pointing straight up |
| **👍** | **Shikhara Mudra** | Clenched fist with thumb pointing upward |

---

## 🛠 Tech Stack & Architecture

- **Client-Side Computer Vision:** Google MediaPipe Tasks Vision (`@mediapipe/tasks-vision`) running on WebAssembly & WebGL.
- **Deterministic Geometric Classifier:** Computes 3D landmark Euclidean distances and finger extensions for forgiving, lag-free recognition in standard room lighting.
- **Render Engine:** High-performance HTML5 Canvas particle system (sparks, embers, smoke) + CSS hardware-accelerated transforms.
- **Audio Synthesis:** Native **Web Audio API** multi-layer procedural synthesizer (sub-bass thumps, demon roars, resonant shimmers) — zero external `.mp3` files required!
- **Zero Build Tools Required:** Pure vanilla JavaScript / HTML5 / CSS3. Runs out-of-the-box in any modern browser.

---

## 🚀 How to Run Locally

1. **Clone the repository:**
   ```bash
   git clone https://github.com/rohitsaidev-art/curse-of-the-mudradhaar-game-anti-gravity.git
   cd curse-of-the-mudradhaar-game-anti-gravity
   ```

2. **Start a local HTTP server:**
   *(Webcams require `http://localhost` or `https://` due to browser security restrictions on `file://`)*
   ```bash
   python3 -m http.server 8080
   ```

3. **Open in your browser:**
   ```
   http://localhost:8080
   ```

4. Click **`⛶ FULLSCREEN`**, allow camera access, and click **"Commence Ritual ⚔️"**!

---

## ⌨️ Keyboard Fallback Controls

If testing in low light or without a webcam:
- **Left Hand:** `1` (🤘), `2` (🖐), `3` (✊), `4` (✌️), `5` (☝️), `6` (👍)
- **Right Hand:** `7` (🤘), `8` (🖐), `9` (✊), `0` (✌️), `-` (☝️), `=` (👍)
- **Restart / Play Again:** `Spacebar`

---

## 📜 License
MIT License. Built with ❤️ on Google Antigravity.
