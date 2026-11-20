# Taiwan ATC Simulator v0.5

Responsive browser-based ATC training prototype. Desktop-first VATSYS-inspired layout with tablet and mobile layouts.

## v0.5 features
- Airport profiles: RCTP, RCKH, RCSS, RCMQ, Taiwan FIR/TMA (all diagrams/data are schematic)
- DEL / GND / TWR / APP / CTR training positions
- Generated sample traffic, flight progress strips, filters and selected-flight data
- Basic command parser and phase workflow controls
- Editable route annotation for each selected flight
- Target selection, drag-to-reposition, map pan and zoom
- Screen-space proximity notices for demo targets (not real separation alerts)
- JSON scenario export/import
- Voice input when browser support and microphone permissions are available
- Responsive desktop / tablet / mobile layout

## Run
Open `index.html` in a modern browser. For microphone support and best compatibility, serve via HTTPS or localhost.

## Publish the static client
Upload `index.html` to the root of a GitHub repository and enable GitHub Pages from Settings -> Pages -> Deploy from a branch -> main -> /(root).

## Multiplayer status
This version remains a single-browser simulation. Real multi-controller synchronization needs a hosted backend and authenticated real-time messaging. The browser WebSocket API supports two-way client/server communication, but it does not create a server by itself. See MDN WebSocket documentation: https://developer.mozilla.org/en-US/docs/Web/API/WebSockets_API

## Safety and data limitations
Training/demo use only; not suitable for real navigation, flight operations or air traffic control. Airport diagrams, runway/taxiway geometry, frequencies, SID/STAR labels, flight plans, movement, clearances and alert logic are illustrative and not validated against current official AIP, NOTAM, aerodrome charts, real flight data or operational separation standards.
