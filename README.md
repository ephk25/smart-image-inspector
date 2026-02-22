# Smart Image Inspector 🔍

A high-performance Chrome Extension (Manifest V3) that leverages Computer Vision to identify and label products within any web image in real-time.

## 🚀 The Mission
Built as a "Micro-Project" to demonstrate API integration, DOM manipulation, and coordinate mapping. Instead of a bloated shopping app, this focuses on the **Core Intelligence**: identifying objects and mapping them to the UI with precision.

## 🛠️ Tech Stack
- **Frontend:** TypeScript, Vite (Build Tool)
- **API:** Google Cloud Vision (Object Localization)
- **UI:** HTML5 Canvas (Bounding Box Overlay)

## 🏗️ Architecture
The extension follows a decoupled logic flow:
1. **Content Script:** Detects image hover and extracts source URLs.
2. **Service Worker:** Handles secure API calls to Google Cloud Vision to bypass CORS.
3. **Canvas Layer:** An invisible overlay is injected to draw the `localizedObjectAnnotations` returned by the AI.


## 📈 Pro Signals
- **Feature Branching:** View the Pull Request history to see the iterative development process.
- **Type Safety:** Built with TypeScript to ensure robust data handling from API responses.
- **Performance:** Optimized canvas rendering to prevent layout shift (CLS).

## 🛤️ Future Roadmap
- [ ] Integration with SerpApi for real-time price comparison.
- [ ] Filter results by "Shop" or "Review Rating."
- [ ] Support for lazy-loaded images. 
