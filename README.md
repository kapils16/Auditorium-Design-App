# Auditorium Design Calculators

A suite of interactive, web-based tools for Architects and Students to calculate, visualize, and optimize auditorium layouts in real-time. This repository contains two standalone tools: one for **Plan/Proportion** design and one for **Sectional Rake** calculation.

Designed to simplify the complex geometry involved in theater acoustics and sightline analysis.

## 🚀 Quick Start

These tools are built with vanilla HTML5, CSS, and JavaScript. They require no installation, build steps, or servers.

1. **Download** the `.html` files.
2. **Open** them directly in any modern web browser (Chrome, Firefox, Edge, Safari).

---

## 🛠 Tool 1: Auditorium Proportions Calculator (Plan View)

**Filename:** `AuditoriumProportionsCalculator.html`

This tool assists in defining the horizontal limits of an auditorium based on the Proscenium arch width. It visualizes the critical 30° and 60° viewing zones and calculates the seating capacity based on the "fan" or "shoebox" geometry.

### Key Features

* **Dynamic Geometry:** Adjust the Proscenium Width, Stage Depth, and the 'P' Ratio (Center point for curved seating) to see changes instantly.
* **Visual Constraints:**
* **30° Line:** Indicates the maximum comfortable viewing depth.
* **Blind Spots:** Automatically hatches areas on stage that are not visible to side seats.
* **110° Limit:** Visualizes the maximum horizontal viewing angle.


* **Row Overlays:** Toggle between visual guides for straight rows or concentric (curved) rows centered on Point P.
* **Smart Stats:** Real-time calculation of:
* Seating Area (m²)
* Estimated Capacity (based on 0.5 m²/person)
* Row widths at the front and back.


* **Angle Probe:** A specialized mouse tool to measure the viewing angle to the proscenium from any point on the canvas.

### Controls

* **Pan:** Click and drag the canvas to move around.
* **Zoom:** Use the mouse wheel to zoom in/out.
* **Probe:** Switch the "Mouse Tool" to "Angle Probe" to inspect specific viewing angles.
  
  <img width="1912" height="1022" alt="image" src="https://github.com/user-attachments/assets/98a60d6d-7678-47f0-85e5-fec54a0a54b6" />
  Screenshot of the Auditorium Proportions Calculator


---

## 📐 Tool 2: Auditorium Section Optimizer (Rake Calculator)

**Filename:** `AuditoriumRakeCalculator.html`


This tool calculates the vertical "Rake" (slope) of the seating tiers. It ensures that every spectator has a clear sightline over the head of the person in front of them to the focal point on stage.

### Key Features

* **Sightline Formula Implementation:** Uses the standard iterative ray-trace method to generate the section profile:



*Where  is the clearance value (typically 120mm) and  is the focal point height.*
* **Safety Checks:** Includes a built-in warning system if the rake angle exceeds **30°**, indicating a need for railings or a balcony split.
* **Parametric Inputs:**
* **C-Value:** Adjust clearance (60mm - 150mm).
* **Stage Height:** Set the focal point elevation relative to the first row.
* **Row Depth:** Adjust spacing between rows.


* **Visualization:**
* Draws the concrete riser structure.
* Plots eye-level points and sightline rays to the stage focus.
* Displays elevation levels for every row.



### Controls

* **Pan:** Click and drag to move the section view.
* **Zoom:** Mouse wheel to inspect riser details.

  <img width="1907" height="1027" alt="image" src="https://github.com/user-attachments/assets/be1b8712-b49d-4316-a19b-8bc3f43a641d" />
  Screenshot of Rake Calculator


---

## 💻 Tech Stack

* **Core:** HTML5 Canvas API for high-performance 2D rendering.
* **Styling:** CSS3 with CSS Variables for dark-mode UI.
* **Logic:** Vanilla JavaScript (ES6+). No external libraries or dependencies used.

## 📝 License & Credits

* **Author:** Kapil Sinha
* **Usage:** Free for educational and personal use.

---

*Repository maintained by kapils16*
