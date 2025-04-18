# Interactive 3D Solar System Simulation

## Description

This project is an interactive, web-based 3D simulation of our solar system, built primarily using the **Three.js** library. It aims to provide an engaging and educational visualization of the Sun, planets, Earth's Moon, and their movements, incorporating several aspects of orbital mechanics for realism.

The simulation allows users to explore the solar system, learn basic facts about celestial bodies, and control various visual aspects.

## Features

* **3D Visualization:** Renders the Sun, planets from Mercury to Neptune, and Earth's Moon.
* **Realistic Orbits:** Implements elliptical and inclined orbits based on approximate Keplerian orbital elements (semi-major axis, eccentricity, inclination, etc.). *Note: Moon's orbit is currently simplified.*
* **Rotation & Tilt:** Simulates sidereal rotation periods and axial tilts for celestial bodies.
* **Interactive Camera:** Uses `OrbitControls` for intuitive navigation:
    * Rotate view (Left-click drag)
    * Pan view (Right-click drag)
    * Zoom view (Scroll wheel)
* **Click-to-Focus:** Click on a celestial body to smoothly move the camera focus to it.
* **Information Panel:** Displays basic information about the currently focused celestial body.
* **Dynamic Controls:** A UI panel allows users to:
    * Adjust the simulation speed (days per second).
    * Toggle the visibility of orbit lines.
    * Toggle the visibility of the background starfield and distant galaxies.
    * Toggle shadow rendering.
    * Reset the camera to the default view.
* **Lighting & Shadows:** Features a central light source (the Sun) and basic shadow mapping for added depth and realism.
* **Background Elements:** Includes a procedurally generated starfield and representative distant galaxy planes.

## Technology Used

* HTML5
* CSS3
* JavaScript (ES6 Modules)
* **Three.js** (JavaScript 3D library - using version r163 or similar via CDN)

## Setup and Running Locally

1.  **Clone or Download:** Get the project files onto your local machine.
    ```bash
    git clone [https://github.com/FrozenSaturn/three-js-solar-system.git](https://github.com/FrozenSaturn/three-js-solar-system.git)
    cd your-repository-name
    ```

2.  **Run a Local Server:** This project uses JavaScript Modules (`import`), which require it to be served over HTTP(S), not loaded directly from the filesystem (`file:///`). Choose one of the following methods:

    * **Using Python 3:**
        ```bash
        python -m http.server
        # or: python3 -m http.server
        ```
        Then open your browser to `http://localhost:8000` (or the port specified).

    * **Using Node.js:** If you have Node.js installed, use the `serve` package:
        ```bash
        npm install -g serve
        serve .
        ```
        Then open your browser to `http://localhost:3000` (or the port specified).

    * **Using VS Code Live Server:** If you are using Visual Studio Code, install the "Live Server" extension and click "Go Live" from the status bar.

3.  **View:** Navigate to the correct local address in your web browser.

## Controls Summary

* **Mouse Navigation:**
    * **Rotate:** Left-Click + Drag
    * **Pan:** Right-Click + Drag
    * **Zoom:** Scroll Wheel
* **Interaction:**
    * **Focus & Info:** Click on the Sun or a planet.
* **Control Panel (Top Right):**
    * Use sliders and checkboxes to adjust speed and visibility settings.
    * Use the "Reset View" button to return the camera to its starting position.

## Future Improvements (Potential TODOs)

* Implement more accurate orbital calculations for moons (relative to their parent planet).
* Add more celestial bodies (dwarf planets like Pluto, major moons of gas giants, asteroid belt visualization).
* Introduce different scaling modes (e.g., logarithmic distance scale).
* Enhance visuals with atmospheric effects (shaders) and higher-resolution textures/maps.
* Optimize performance further, possibly using Level of Detail (LOD).

---

*(Optional: Add License Information Here, e.g., MIT License)*
*(Optional: Add Author/Contact Information Here)*
