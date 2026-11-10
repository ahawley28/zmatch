# ZMatch — interactive Smith chart matcher

**Open it here:** https://ahawley28.github.io/zmatch/

A single-page, in-browser tool for designing impedance-matching networks on a Smith chart.
Nothing to install — it runs entirely in your browser, and your settings are saved locally.

## Features

- **Smith chart** with zoom/pan; finer r / x (and optional g / b) grid lines appear as you zoom in
- **Matching components:** series/shunt L and C, series transmission lines, open and shorted stubs
- **Drag a component's dot** on the chart to set its value, with gentle snapping to constant-r / constant-g
  circles, the chart center, and line Z₀ / stub Y circles (hold Shift to skip snapping)
- **Microstrip lines** from W, L and the substrate (εr, H, T) — Hammerstad–Jensen or a simple
  377·H/((W+2H)√εr) model — or ideal lines from Z₀ and θ
- **Device models:** fixed R + jX, series R–C, parallel R‖C, series R–L
- **View-frequency slider** (with play) to watch the network detune off the design frequency,
  plus a frequency sweep with a |Γ| vs f plot and −10 dB bandwidth
- Each component shows its **reactance and susceptance**; series lines also show their exact π-model
- **Built-in complex calculator** (uses `j`): editable rows, `||` for parallel, SI suffixes (`33.5f`, `94G`),
  variables, and RF helpers such as `zc(C,f)`, `gam(Z)`, `zline(ZL,Zc,θ)`

## Use

Open the link above, or download `index.html` and open it in any modern browser.
Click **How to use** in the top bar for a quick guide.

---
By Andrew Hawley
