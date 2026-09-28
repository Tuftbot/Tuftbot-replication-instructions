## Tiles generator


Zoe Romano worked on the development of a HTML based software to automatise the design of tufted tiles which export the required files for the robotufting process.
Hexweave is a self-contained, single-file web application written entirely in HTML, CSS, and vanilla JavaScript with no frameworks, no build tools, no dependencies.

The visual interface (layout, controls, typography) is built in HTML5 and styled with CSS3, using CSS custom properties (variables) for the design token system, CSS Grid and Flexbox for the responsive layout, and CSS keyframe animations for the flash ring interaction feedback.

The geometry engine is pure JavaScript (ES2020). It computes a flat-top hexagonal tessellation grid analytically, deriving each tile's centre coordinates, edge midpoints, and outward normal vectors in real time, and renders the Van Ness cord matchings as cubic Bézier curves, with handle lengths scaled proportionally to each chord for consistent curvature across adjacent, skip-1, and opposite edge pairings.

The drawing surface is an SVG (Scalable Vector Graphics) element built dynamically by the JavaScript, which constructs and inserts SVG path elements directly into the DOM on every state change. There is no canvas rasterisation and no pixel data, the entire graphic is resolution-independent vector geometry.

The interactivity, using sliders, dropdowns, single-click rotation, double-click class cycling, and the reshuffle function, is handled through native browser DOM events with no external libraries. The download buttons generate SVG files client-side by encoding the geometry as a data: URI and triggering a programmatic anchor click.

[Here](Files/hexweave_tuftbot_final.html) you can fine the Html file for the Tile generator which you can download and run on your browser.
