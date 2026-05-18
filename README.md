# Dynamic Form Redirection Gateway

A lightweight client-side routing gateway built with HTML, CSS, and JavaScript. This platform was deployed as an intermediate redirect interface for a university student club recruitment drive.

## 💡 The Problem It Solved
When distributing form links via bulk email campaigns, any changes to the target URL normally require resending the communication. This gateway solves that challenge by acting as a fixed proxy layer. If the final form changes, the development team only updates the code inside this gateway repository, ensuring zero broken or outdated links reach the end user.

## 🚀 Technical Implementation
- **Browser Object Model (BOM):** Utilizes `window.onload` to catch page instantiation states and seamlessly pushes destination parameters using `window.location.href`.
- **Asynchronous Scheduling:** Leverages `setTimeout` to manage the transition countdown smoothly.
- **Library Integration:** Integrates external character scripts (`canvas-confetti`) via CDN streams, driving interactive canvas renders inside a custom `requestAnimationFrame` execution frame.

## 🛠️ Stack
- HTML5 / CSS3 (Glassmorphism layout framework)
- Vanilla JavaScript
- Canvas Confetti API (v1.6.0)
