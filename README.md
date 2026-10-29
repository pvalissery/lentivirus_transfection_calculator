# Lentivirus Transfection Calculator 🧬

This is a zero-dependency, single-page web app that handles the math for your transfection master mixes. 
https://pvalissery.github.io/lentivirus_transfection_calculator/

This tool calculates exact volumes for packaging plasmids (psPAX2), envelope plasmids (pMD2.G), and custom transfer plasmids based on your target DNA concentrations and scaling requirements.

## Why this exists
Managing multiple transfer plasmids across different transfection scales usually means endless copy-pasting in spreadsheets. This app moves the workflow to a clean web UI where you can dynamically add plasmids, tweak concentrations, and get an auto-updating Master Mix recipe without the spreadsheet headache. 

## Features
* **Instant Calculations:** Every volume and master mix scale updates in real-time as you type. 
* **Dynamic Plasmid Entries:** Add or remove as many transfer plasmids as you need for a given experiment.
* **Auto-Generated Master Mixes:** Calculates the exact ratios of Opti-MEM, TRANS-LT-1, and your plasmid trio for each specific transfer construct.
* **Responsive Design:** Scales perfectly down to mobile if you're checking numbers on your phone at the bench.
* **Zero Overhead:** No backend, no build steps, no npm installs. It all runs client-side in the browser.

## Tech Stack
* **HTML5 / Vanilla JavaScript:** Keeps the logic fast and entirely client-side.
* **Tailwind CSS (via CDN):** For a clean, readable, and responsive UI without maintaining a massive stylesheet.

## Usage
You don't need to install anything. 

1. Clone this repository or download the source.
2. Double-click `index.html` to open it in any modern web browser.
3. Input your stock concentrations, set your target DNA mass (µg), and add your transfer plasmids. The Master Mix cards will generate at the bottom automatically.

## Future Plans / Caveats
* *Currently hardcoded for the psPAX2 / pMD2.G / TRANS-LT-1 system.* If you use a different generation of lentiviral packaging or a different transfection reagent (like PEI or Lipofectamine), you'll need to fork this and adjust the reagent logic in the JavaScript file.
