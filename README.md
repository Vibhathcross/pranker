# Secure Access Gateway (Interactive Browser Prank)

A highly immersive, single-file browser prank designed to simulate a faux system compromise. Built with vanilla HTML, CSS, and JavaScript, this project uses a three-phase psychological progression (Bait, Trap, Reveal) combined with browser APIs to create a convincing and panic-inducing user experience. 

It is 100% self-contained, requiring no external assets, images, or audio files.

## 🚀 Features

* **Three-Phase Sequence:**
  * **Phase 1 (The Bait):** A benign "Human Verification" screen designed to secure the user interaction required to trigger browser Audio and Fullscreen APIs.
  * **Phase 2 (The Trap):** A fake hacker terminal featuring a realistic typewriter effect, randomized fake IP generation, dynamic progress bars, and CRT monitor styling.
  * **Phase 3 (The Reveal):** A flashing, high-contrast jump scare with CSS animations and CSS-driven glitch effects.
* **Procedural Audio Engine:** Utilizes the Web Audio API to synthesize high-tech terminal beeps and emergency sirens directly in the browser—no `.mp3` or `.wav` files needed.
* **Immersive Fullscreen Trap:** Automatically requests fullscreen mode upon interaction to hide the user's OS taskbar and browser tabs, heightening the panic.
* **Fully Responsive:** Uses CSS `clamp()` functions and viewport units to scale perfectly from ultra-wide desktop monitors to narrow mobile phone screens.
* **Zero Dependencies:** Written entirely in vanilla web languages within a single `index.html` file.

## 🕹️ Secret Escape Hatches (Admin Overrides)

To prevent users from being permanently trapped, the system includes hidden loopholes. If a user panics and triggers one of these escapes, the alarms stop, fullscreen exits, and they are rewarded with an "Admin Override" visual theme (`hue-rotate` and `invert` CSS filters).

* **Desktop (Keyboard Panic):** * Press the `ESCAPE` key 3 times rapidly.
  * *Or* type the words `STOP`, `EXIT`, or `HELP`.
* **Mobile (Touch Panic):** * Tap anywhere on the screen 5 times rapidly (within 2 seconds).

## 🛠️ Usage

1. Clone or download this repository.
2. Open the `index.html` file in any modern web browser (Chrome, Firefox, Safari, Edge).
3. Click "Verify & Enter" to begin the sequence.

## 💻 Technical Highlights

* **Memory Management:** The desktop keylogger uses a rolling string buffer (`substring()`) capped at 15 characters to prevent memory leaks during continuous typing.
* **Mobile Touch Optimization:** Implements `touch-action: manipulation;` to disable native double-tap-to-zoom behaviors, ensuring the rapid 5-tap mobile escape hatch registers accurately.
* **Asynchronous Timing:** Heavily utilizes nested `setTimeout` and `setInterval` functions to pace the user experience and build suspense.

## ⚠️ Disclaimer

This project is intended for **educational and entertainment purposes only**. Do not use this to harass, bully, or genuinely distress individuals. The creator is not responsible for any dropped phones, spilled coffee, or panic attacks resulting from the use of this software.
