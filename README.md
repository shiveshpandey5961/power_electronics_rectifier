# power_electronics_rectifier ⚡

An interactive, browser-based power electronics laboratory for simulating, visualizing, and analyzing **diode (DBR)** and **thyristor (TCR)** rectifiers in real time.

Live interactive waveforms, closed-loop current flow visualization, active device illumination, and steady-state theoretical verification.

---

## 🚀 Key Features

* **Multiple Converter Topologies:**
  * Single-phase Half-wave & Full-wave Bridge
  * Three-phase Half-wave (3-pulse) & Full-wave Bridge (6-pulse)
* **Devices Supported:**
  * Uncontrolled Diode Bridge Rectifiers (DBR)
  * Phase-Controlled Thyristor Rectifiers (TCR) with firing angle $\alpha \in [0^\circ, 180^\circ]$
* **Loads & Commutation:**
  * Pure Resistive ($R$)
  * Inductive ($R-L$)
  * Back-EMF Battery / DC Motor load ($R-L-E$)
  * Freewheeling Diode (FWD) support
* **Interactive Circuit Visualizations:**
  * **Dynamic Current Flow Path:** Animated directional chevrons show the closed-loop path of circulating current through the supply, converter devices, and load.
  * **Device Illumination & Dimming:** Conducting devices glow with active halos; non-conducting devices dim out to eliminate clutter.
  * **Gate Pulse Indicators:** Gate terminal indicators illuminate at firing instants.
  * **Local Freewheeling Loop:** Highlights the circulating path through the freewheeling diode when the AC supply is disconnected.
* **Waveform Studio:**
  * Output voltage $v_o(t)$, load current $i_o(t)$, and source voltages $v_s(t)$ plotted over a full cycle.
  * Interactive scrub cursor with hover tooltip showing instantaneous electrical values.
  * Conduction interval timeline and thyristor firing markers.
  * Play, Pause, speed multipliers ($0.25\times, 0.5\times, 1\times, 2\times$), and step buttons ($◀ -5^\circ$, $+5^\circ ▶$).
* **Steady-State Metrics & Analytical Verification:**
  * $V_{dc}$ (Mean output voltage)
  * $V_{rms}$ (RMS output voltage)
  * $I_{dc}$ and $I_{rms}$
  * Peak load current $I_{\text{peak}}$
  * Ripple Factor ($V_{ac,rms} / V_{dc}$)
  * Form Factor ($V_{rms} / V_{dc}$)
  * Absorbed Load Power ($I_{rms}^2 R + E I_{dc}$)
  * Rectification Efficiency $\eta$
  * Conduction angle
  * Analytical Textbook $V_{dc}$ formula verification
  * Peak Inverse Voltage (PIV) rating
* **Zero Dependencies:** Pure HTML5 Canvas, modern CSS, and vanilla JavaScript in a single self-contained file.

---

## 💻 How to Run Locally

Simply double-click `index.html` (or `rectifier-bench.html`) to open it in any modern browser (Chrome, Edge, Firefox, Safari). No installation, servers, or build tools required!

---

## 🌐 Deploy to GitHub Pages (Free Live Web URL)

1. Push this repository to GitHub.
2. Go to **Settings** > **Pages** in your repository.
3. Under **Branch**, select `main` (or `master`) and `/ (root)`.
4. Click **Save**.
5. Your interactive rectifier bench will be live at:
   ```
   https://<your-username>.github.io/<your-repo-name>/
   ```

---

## 📜 License
MIT License. Open for educational and research use.
