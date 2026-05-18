# Dynamic Form Redirection Gateway

An intermediate proxy and presentation gateway page built using HTML5, CSS3, and interactive client-side JavaScript. This platform was deployed as a proxy routing interface for a university student club recruitment drive.

---

## 👤 Developer Profile
- **Name:** Vaibhav Mishra
- **Drive Context:** Cognizant Digital Nurture 5.0 (Java FSE Track)

---

## ⚠️ Important Note for Code Reviewers
When launching the live project deployment, the browser executes an automatic **2.5-second asynchronous routing loop** managed entirely by JavaScript before passing control over to an external Google Form. 
- **The Logic:** This intermediary buffer solves link deprecation layout issues in bulk email setups, allowing the backend pointer to change inside this codebase without needing to alter sent URLs.
- **What to Observe:** Upon load, watch for the immediate instantiation of third-party canvas stream particles followed by an explicit Browser Object Model (BOM) redirection command.

---

## 💡 The Problem It Solved
When distributing form links via bulk email campaigns, any changes to the target URL normally require resending the communication. This gateway solves that challenge by acting as a fixed proxy layer. If the final form changes, the development team only updates the code inside this single gateway repository, ensuring zero broken, outdated, or dead links reach the end user.

## 🚀 Technical Implementation & Script Features
- **Browser Object Model (BOM):** Connects to the window lifecycle via `window.onload` to handle initial mounting behaviors cleanly and seamlessly pushes destination parameters using `window.location.href`.
- **Asynchronous Scheduling:** Leverages the `setTimeout` window timer API to manage a strict 2500-millisecond countdown transition smoothly before triggering the redirection execution state.
- **High-Performance UI Animation:** Integrates external character scripts (`canvas-confetti`) via CDN streams, driving interactive canvas renders inside custom `requestAnimationFrame` execution frames to keep visual animations completely decoupled from the main operational runtime pipeline.

## 🛠️ How to Update the Target Form Link
To change the destination address of the redirection system, update the execution path parameter located inside the script block at the bottom of the main index file:

```javascript
// Locate this block at the bottom of the source file to change the routing target:
setTimeout(function() {
    window.location.href = "YOUR_UPDATED_FORM_LINK_HERE"; 
}, 2500);
