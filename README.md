# 🕯️ Contract with the Machine (Digital Séance)

![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E)

> **An official submission for the IEEE Prankraft Competition.** > *A psychological UI/UX prank that transforms a standard registration form into an immersive, cinematic, and deeply unsettling "digital séance."*

🔗 **[Play the Live Demo Here] (Insert your Netlify/GitHub Pages link here)**

---

## 👁️ The Concept

Most frontend pranks rely on simple "broken" features or jump scares. *Contract with the Machine* moves beyond simple frustration and creates a psychological trap. It looks like a high-end, luxury registration form, but the UI is "possessed" by a ghost in the code. 

The user is drawn into a cat-and-mouse game where the interface actively gaslights them, evades them, and watches them.

---

## 🕸️ Core Features

### 1. The "False Security" Trap (Delayed Activation)
The website initially behaves completely normally to build trust. The mouse works fine, and the buttons remain stationary. The "Ghost" only awakens once the user commits to the action by typing their first character. The user feels responsible for "waking up" the anomaly.

### 2. Loss of Agency (The Repelling Button)
In standard web design, the user is the "God" of the interface. This prank subverts that power.
* **The Mechanic:** A custom Repel Algorithm calculates the distance between the cursor and the submit button. As the user gets closer, the button uses a physics-based "push" to glide away.
* **The Psychology:** It creates an engaging cat-and-mouse game. Because the button smoothly returns to its original spot when the user retreats, it visually "dares" the user to try again.

### 3. Digital Gaslighting (Possessed Text)
This targets the user's trust in their own input.
* **The Mechanic:** As the user types their email, an inactivity tracker monitors their cadence. If they pause for too long, the screen blinks, and their typed text is abruptly swapped with a "Ghostly Dialogue" (e.g., *"I am watching you"*).
* **The Execution:** Using dynamic "Zalgo" text injection, the input visually decays, making the browser look physically corrupted.

### 4. Atmospheric Immersion & Web Audio API
To meet high UI/UX design standards, the prank utilizes cinematic techniques:
* **Visuals:** A Vantablack color palette, CSS film grain noise, and a "breathing" vignette effect that pulses around the edges of the screen to create claustrophobia.
* **Audio:** Powered by the **Web Audio API**, the site generates a low-frequency, binaural hum. As the user's mouse nears the elusive submit button, the frequency and volume increase, subconsciously raising the user's anxiety.

### 5. The Fourth Wall Break (Phantom Shadows)
Custom, blurred CSS radial gradients spawn dynamically and drift across the screen. They occupy the user's peripheral vision, creating the illusion that the "Ghost" isn't just in the code, but is a physical presence behind the glass of the monitor.

### 6. The Escape Hatch (The Exorcism)
Every good prank needs a user-friendly solution. 
* **The Puzzle:** A hidden, nearly invisible icon (⚲) rests in the top right corner of the screen.
* **The Cleanse:** When clicked, it triggers a "Holy Flash." All CSS variables revert, the Zalgo text is purged, system fonts replace the gothic serifs, and the physics engine is disabled. The user is finally allowed to submit the form in peace.

---

## 🛠️ Tech Stack & Implementation Details

* **Vanilla JavaScript (ES6+):** No external frameworks or physics libraries were used. The repel math, Zalgo text generation, inactivity timers, and state management are built from scratch.
* **CSS3:** Heavy use of `transform` for hardware-accelerated animations, `filter: blur()` for shadows, and `clip-path` / `radial-gradient` for atmospheric rendering.
* **Web Audio API:** Used to create a dynamic `OscillatorNode` (Triangle/Sawtooth waves) tied to mouse distance calculations for interactive sound design.

---

## 🚀 How to Run Locally

1. Clone the repository:
   ```bash
   git clone [https://github.com/YourUsername/digital-seance.git](https://github.com/YourUsername/digital-seance.git)
