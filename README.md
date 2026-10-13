# ERA — Emergency Response Web Prototype

A refreshed React + Vite UI for the Emergency Response Application (ERA). This is a frontend-only prototype with local demo data; it does not contact real emergency services.

## Included in this package

- Responsive dashboard for desktop, tablet, and mobile screens
- Bright emergency-inspired palette: midnight navy, signal coral, cyan, teal, amber, and violet
- Animated SOS hero treatment, pulsing location pins, an animated route line, floating visual indicators, and modal/toast transitions
- Scroll-triggered reveal animations using the browser's `IntersectionObserver`
- Navigation for Overview, My emergencies, Live tracking, Medical profile, Responder view, and Messages
- Simulated SOS request flow and searchable emergency history
- Responsive illustrative map (not a live map)
- No icon library dependency: the interface icons are inline SVG, reducing the risk of third-party icon import errors
- Clear setup and troubleshooting steps

## Requirements

- Node.js 18 or newer
- npm
- VS Code or another code editor

## Run locally on Windows

1. Download and extract `ERA-Web-Prototype-Redesigned.zip`.
2. Open the extracted `era-web-redesign` folder in VS Code.
3. Select **Terminal → New Terminal**.
4. Run:

   ```bash
   npm install
   npm run dev
   ```

5. Open the `Local` URL printed in the terminal (usually `http://localhost:5173`).

To make a production build, run:

```bash
npm run build
```

The generated site will be placed in `dist/`.

## If the preview is blank

- Confirm you opened the project root — the same folder that contains `package.json`, `index.html`, and `src/`.
- Run `npm install` from that folder and wait for it to complete.
- Run `npm run dev` and open the exact `Local` URL shown in the terminal. Avoid opening `src/App.jsx` or `index.html` directly as a local file.
- Read the first red error in the terminal or browser developer console. If the preview still appears blank, copy that first error message when asking for help.
- If your editor has a separate **Preview** panel, restart/reload the preview after dependencies finish installing.

## Project structure

```text
era-web-redesign/
├── index.html
├── package.json
├── vite.config.js
├── README.md
└── src/
    ├── App.jsx
    ├── main.jsx
    └── styles.css
```

## Demo-only safety note

- SOS submissions are stored only in React page state. No call or message is sent to emergency responders.
- The displayed Ruiru map, route, and responder markers are illustrative and do not use GPS or live maps.
- Medical profile values are not securely persisted or sent to a server.
- The responder accept button only changes local demo state.
- Do not rely on this prototype for real emergencies. Production use would require secure authentication, consent and privacy controls, a backend, validated geolocation, reliable notifications, monitoring, and real-world testing with authorized emergency service partners.

## Repository

GitHub project: https://github.com/Ngignjeri/ERA-Emergency-Response-
