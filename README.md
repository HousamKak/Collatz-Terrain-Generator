## Collatz Terrain Generator

A static web application that transforms Collatz sequence values into procedurally generated 2D terrain visuals. Built with vanilla JavaScript, HTML, and CSS, this project showcases advanced noise-based terrain generation combined with Collatz sequence analysis.

---

### 🚀 Live Demo

View the application live on GitHub Pages: [YourUsername.github.io/CollatzTerrain](https://YourUsername.github.io/CollatzTerrain)

---

## 📋 Features

* **Procedural Terrain Generation**: Utilizes simplex noise and Collatz sequence values to create unique terrain for any seed input.
* **Interactive Controls**:

  * **Seed**: Specify any positive integer to generate a corresponding Collatz terrain map.
  * **Scale & Octaves**: Adjust noise frequency and detail levels.
  * **Quality Settings**: Toggle between low, normal, and high resolution.
  * **Color Palettes**: Switch between classic, volcanic, alien, and autumn themes.
* **Collatz Analysis**:

  * **Sequence Display**: See the partial or full Collatz sequence for the current seed.
  * **Statistics**: Auto-calculated sequence length, maximum value, complexity, and volatility.
  * **Sparkline Chart**: Visualize sequence fluctuations.
* **Export Options**:

  * **Save Terrain Image** (PNG)
  * **Download Heightmap** (Grayscale PNG)
  * **Export Sequence Data** (JSON)
* **Shareable URLs**: Generate and copy a URL that encodes current parameters for easy sharing.
* **Responsive Layout**: Adapts to various screen sizes with CSS Grid and Flexbox.

---

## 🛠️ Getting Started

Follow these instructions to get a local copy up and running.

### Prerequisites

* A modern web browser (Chrome, Firefox, Safari, Edge).
* Git (optional, for version control).

### Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/YourUsername/CollatzTerrain.git
   cd CollatzTerrain
   ```

2. **Deploy to GitHub Pages**

   * Push the code to a GitHub repository named `CollatzTerrain`.
   * In repository settings, enable GitHub Pages, selecting the `main` branch and `/ (root)` folder.

3. **Or run locally**

   * Open `index.html` in your browser.

---

## 🎮 Usage

1. **Seed Configuration**

   * Enter a positive integer in the Seed field.
   * Click **Generate** to build the terrain.
   * Use **Random** for a random seed.

2. **Animation Mode**

   * Click **Animate** to cycle through Collatz-derived seeds automatically.

3. **Adjust Terrain**

   * **Scale**: Modify base noise frequency.
   * **Octaves**: Increase or decrease terrain detail.
   * **Quality**: Select resolution vs. performance.

4. **Palette & Legend**

   * Choose a color palette in the sidebar.
   * Hover legend items to see elevation thresholds.

5. **Export**

   * **Save Image**: Downloads a PNG of the terrain view.
   * **Heightmap**: Downloads a grayscale heightmap PNG.
   * **Export Data**: Downloads JSON with sequence and parameters.

6. **Sharing**

   * Click **Share** to generate a URL encoding all parameters.
   * Copy the link to revisit or share your custom terrain.

---

## ⚙️ Configuration

All configurable parameters are defined in `script.js` under the `CONFIG` object:

```js
const CONFIG = {
  TERRAIN: { /* size & thresholds */ },
  ANIMATION: { /* throttle & intervals */ },
  PALETTES: { /* color definitions */ }
};
```

* **Add New Palettes**: Extend the `PALETTES` object with new color arrays.
* **Modify Thresholds**: Tweak elevation cutoffs in `TERRAIN.ELEVATION_THRESHOLDS`.

---

## 🤝 Contributing

Contributions are welcome! Please fork the repository, create a feature branch, and submit a pull request.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📜 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

*Enjoy exploring the nexus of mathematics and procedural art!*
