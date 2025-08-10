# Bloom Filter Explainer

Interactive, single-page demo illustrating how Bloom filters work. Adjust parameters, insert or query values, and watch hash probes light up on a canvas.

## Features
- Tune bit array size `m` (64–4096) and number of hash functions `k` (1–10) with sliders
- Optional per-hash tracing with adjustable speed, plus an estimated false positive curve
- Add values manually or randomly, check membership, and clear the filter while metrics update in real time
- Visual legend and keyboard shortcuts for quick interaction (R random, A add, C check, X clear, H toggle help, ? overlay)

## Usage
Open `BloomFilterExplainer.html` in any modern browser. No build step or server is required.

## Implementation
The demo uses an in-browser `Bloom` class to manage the bit array, hash calculations, and false-positive estimation. All rendering is done via the HTML5 Canvas API with lightweight vanilla JavaScript.
