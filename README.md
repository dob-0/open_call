# WCC - Unified Campaign Engine (Open Call & Talks Hub)

A lightweight, single-file React and Three.js application designed for the **Women Creating Change (WCC)** contemporary art initiative. This platform serves as a digital hub for Open Calls, Event/Talk promotions, and application processing.

## 🚀 Features
* **Zero-Build Architecture:** The entire application (React, Tailwind CSS, Three.js, Babel) runs entirely from a single `index.html` file. No Node.js, Webpack, or NPM required.
* **Interactive 3D Environment:** Features a generative WebGL background built with Three.js that responds to user configuration.
* **Hidden Admin Dashboard:** A built-in, secure control panel for live-editing the website.
* **Native Form Mapper:** Automatically parses and maps Google Forms URLs into a beautiful, custom-styled native UI (bypassing ugly iFrames).
* **Export Engine:** Built-in tools to capture high-resolution HTML5 Canvas PNG posters and record WebM video reels for Instagram/TikTok marketing.
* **Local First:** All form submissions are backed up locally in the browser and can be exported as a CSV.

## 🛠️ How to Access the Admin Panel
The website contains a hidden Developer/Admin dashboard used to modify the content, colors, and 3D shapes.

To access it on any device, use one of the following methods:
1. **Desktop:** Press the `H` key on your keyboard.
2. **Mobile/Touch:** Triple-tap the extreme **bottom-left corner** of the screen rapidly.

*(Note: The Admin Panel modifies local browser state. To make changes permanent for all users, see the deployment steps below).*

## 📖 How to Update the Live Website
Because this project uses no backend database, updating the live website is done via HTML generation.

1. Open the website and access the **Admin Panel**.
2. Make your desired changes (update copy, change colors, upload speaker photos, etc).
3. Navigate to the **Export Posters & Video** menu.
4. Click **Download Configured HTML**. This will download a new `index.html` file containing your new default settings.
5. Replace the `index.html` file in your Git repository with this new file.
6. Commit and push to your `main` branch.

## 🐛 Debugging & Logs
To access the hidden system developer console, press the `D` key on your keyboard. This will open a terminal overlay showing form-mapping logs, Google fetch requests, and system errors.

## 🎨 Graphic Design & Export Guidelines
The app includes a graphic design engine to generate promotional posters directly from the 3D scene.
* **Standard Post:** Set export dimensions to `1080x1350`.
* **Story/Reel:** Set export dimensions to `1080x1920`.
* Use the "Artwork Composition" sliders in the Admin panel to frame the 3D art properly before clicking "Poster Layout (PNG)".

## ⚖️ License
This project is released under the **CC0 1.0 Universal (Public Domain Dedication)** license. You can copy, modify, and distribute the work, even for commercial purposes, without asking permission.
