# Bunv

**Bunv** is a lightweight, blazing-fast, and developer-friendly cross-platform desktop application bundler built with **Bun** and **Webview**. It empowers frontend developers to build, debug, and package native desktop apps using pure JavaScript/TypeScript and web technologies—offering a compelling alternative to Electron and Tauri with smaller bundle size and faster startup.

## Features

- **Minimal footprint:** Bundled apps typically range from 5MB to 60MB, significantly smaller than Electron-based apps.
- **Super fast startup:** Thanks to Bun’s high-performance JavaScript runtime and native Webview rendering.
- **Familiar web tech:** Use HTML, CSS, and TypeScript/JavaScript to build your UI and app logic.
- **Seamless system API access:** Easily extend system integrations like clipboard, file dialogs, notifications via Bun’s native bridge.
- **Simple bundling:** One command bundles your app into a native executable for Windows/macOS/Linux.
- **Easy scaffolding:** Start a new project with a simple CLI, no complex Rust or C knowledge needed.

## Why Bunv?

| Feature                   | Electron           | Tauri                          | Bunv (Bun + Webview)        |
| ------------------------- | ------------------ | ------------------------------ | --------------------------- |
| **Runtime**               | Node.js + Chromium | Rust + Webview                 | Bun + Webview               |
| **Bundle size**           | 100MB+             | 5-30MB                         | \~5-60MB                    |
| **Startup speed**         | Moderate           | Fast                           | Very fast                   |
| **Development stack**     | JS/Node + web tech | Rust + web tech                | Pure JS/TS + web tech       |
| **Complexity**            | Medium             | High (Rust knowledge required) | Low (only JS/TS and Bun)    |
| **Cross-platform**        | Yes                | Yes                            | Yes                         |
| **System APIs**           | Rich, but large    | Rich, Rust-powered             | Growing, JS + native bridge |
| **Community & Ecosystem** | Mature, large      | Growing, smaller               | Emerging, innovative        |

## Inspiration

Bunv draws inspiration from:

- [Electron](https://www.electronjs.org/): The most popular desktop app framework, providing rich APIs but heavyweight.
- [Tauri](https://tauri.app/): A Rust-based, lightweight alternative with excellent system integration but steep learning curve.
- [webview-bun](https://github.com/tr1ckydev/webview-bun): Demonstrated the power of Bun + Webview for desktop apps with high performance and small size.

Bunv aims to combine the best of these worlds: **speed, simplicity, and small size**—while fully embracing JavaScript/TypeScript and modern web tooling.

## Roadmap

- [ ] Core Bun + Webview integration to launch native windows
- [ ] Basic JS/TS bridge for calling system APIs (clipboard, file dialogs, notifications)
- [ ] Simple CLI scaffolding for new projects
- [ ] Cross-platform build pipeline for Windows/macOS/Linux
- [ ] Advanced system API wrappers (tray, shortcuts, multi-window support)
- [ ] Plugin system to extend Bunv’s capabilities easily
- [ ] Rich documentation and examples
- [ ] Continuous integration & automated releases

## Getting Started

```bash
bun create Bunv my-app
cd my-app
bun run build
```

## Contribution

Contributions are welcome! Feel free to open issues or submit pull requests.

## License

MIT License
