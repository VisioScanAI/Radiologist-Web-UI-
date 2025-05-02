# VISIOSCAN AI - MVP Radiologist Web UI

## Directory Structure
```
visioscan_webui/
├── README.md
├── package.json
├── webpack.config.js
├── public/
│   └── index.html
├── src/
│   ├── index.jsx
│   ├── App.jsx
│   ├── viewmodels/
│   │   └── ImageViewerViewModel.js
│   ├── components/
│   │   └── ImageViewer.jsx
│   ├── services/
│   │   └── api.js
│   └── extensions/
│       └── visioscan-extension/
│           ├── manifest.json
│           ├── index.js
│           └── extensionConfig.js
```

--- README.md ---
# VISIOSCAN AI - Radiologist Web UI

A stateless single-page application (SPA) built as an OHIF extension to integrate within any PACS. Implements MVVM with functional React components and viewmodels for real-time AI inference overlays.

## Features
- **CXR & Head CT viewer:** DICOM image series browsing via OHIF
- **AI overlay:** Real-time pathology detection results rendered atop images
- **MVVM architecture:** Separation of UI (components) and state logic (viewmodels)
- **Stateless design:** No local state persistence; all data fetched on-the-fly
- **OHIF Extension:** Plug-and-play manifest for easy PACS integration

## Tech Stack
- React 18
- Vite + Webpack for bundling
- RxJS for reactive viewmodel streams
- OHIF Extension API
- Axios for HTTP
