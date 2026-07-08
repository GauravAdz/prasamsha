# 🌸 For Prasamsha — A Digital Love Letter & Apology

> **Note to fellow developers:** If you stumbled upon this repo looking for a way to impress your girlfriend, apologize for being an idiot, or just do something completely over-the-top for an anniversary—this is how you do it. This project is a highly personalized, 10-chapter interactive web experience built to say "I'm sorry" and "I love you" through code. Feel free to fork it, study it, and adapt it for your own person.

This project is a single-file, dependency-free interactive webpage designed for a specific person. It takes the user on a journey through different "chapters," featuring interactive elements, mini-games, and personalized messages.

## 🔗 Live Demo
You can view the live project here:  
👉 **[mylove.gauravadhikari.info.np](https://mylove.gauravadhikari.info.np)**

## ✨ Features

This isn't just a static page; it's heavily interactive. Here is a breakdown of the "chapters":

* **✉️ Interactive Envelope:** A CSS-animated envelope that opens when tapped, triggering falling petals and background music.
* **🗺️ Animated Bridge Map:** A custom SVG map connecting two cities (Linz and Southampton) with a glowing, animated path and a hidden message.
* **🕰️ Dual Clocks:** Live, dual-timezone clocks keeping track of our two locations.
* **📅 Relationship Timeline:** An expandable, interactive timeline of important dates and milestones.
* **🎴 "Open When" Cards:** 3D CSS flip-cards with personalized messages for different moods/situations.
* **🌱 Interactive Garden:** Tap the screen to plant dynamically generated CSS flowers, each revealing a reason why I like her.
* **📸 Polaroid Stack:** A swipeable, physics-based stack of polaroids (supports both images and looping videos).
* **🎸 Draggable Record Player:** An interactive vinyl player. Drag the tonearm onto the record to fade out the background music and play "her song."
* **🩺 Mood Decoder:** A dynamic "prescription" generator based on how she is currently feeling.
* **🕹️ 8-Bit Canvas Quest:** A custom HTML5 Canvas mini-game where the player jumps over "storm clouds" (arguments) to collect hearts and reach the end.
* **💖 Press-and-Hold Finale:** A final CSS/JS animation that stretches out her name the way I type it when she holds down a heart button.

## 🛠️ Tech Stack

Built completely from scratch. No frameworks, no libraries, no npm installs.
* **HTML5:** Semantic structure and layout.
* **CSS3:** Custom properties, complex keyframe animations, 3D transforms, and responsive design (mobile-first).
* **Vanilla JavaScript (ES6):** DOM manipulation, HTML5 Audio API for smooth track crossfading, multi-touch event handling for the record player and final heart, and a custom physics loop for the Canvas mini-game.

## 🚀 How to Run Locally

Because this is vanilla web tech, you don't need a build step. 

1. Clone the repository.
2. Ensure you add the required media assets to the root directory (see **Required Assets** below).
3. Double-click `index.html` to open it in your browser, or use an extension like VSCode Live Server for the best experience.

### 📂 Required Assets
To make this work locally without broken links, you need to add a few of your own files into the same folder as `index.html`:

* **Audio:** 
    * `the-man-who-cant-be-moved.mp3` (Background track)
    * `go-away-weezer.mp3` (Vinyl record track)
* **Images/Video (for the map and polaroids):**
    * `her-face.png`
    * `my-face.jpeg`
    * `photo1.png`, `photo2.png`, `photo4.png`
    * `0707.mov`, `7071.mp4` *(Yes, the polaroids support looping, muted video!)*

## 🔧 How to Customize It for Your Person

If you are using this as a template to impress your partner, here is where you need to look in the code:

1.  **The Names:** Search the file for `Prasamsha` and `Gaurav` and replace them.
2.  **The Map (Chapter 1):** Find the `<svg id="bridgeSvg">` block. You can change the city labels, the `cx` and `cy` coordinates of the face pins, and the SVG path to match your own geographic distance.
3.  **The Timeline (Chapter 3):** Edit the `<div class="tl-item">` blocks to reflect your own milestones.
4.  **The Garden Reasons (Chapter 6):** Find the `const REASONS = [...]` array in the `<script>` section and replace it with your own list.
5.  **The Polaroids (Chapter 7):** Find `const PHOTOS = [...]` in the `<script>` tag. Update the filenames and captions to match the photos/videos you dropped into the folder.
6.  **The Prescription (Chapter 9):** Edit the `const RX = {...}` object in the script to write your own responses for their moods.

---
*Built with HTML, CSS, JS, and a lot of feelings.*
