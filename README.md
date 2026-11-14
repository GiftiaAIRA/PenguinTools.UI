# PenguinTools.UI Extend

PenguinTools Extend is a fork of [PenguinTools.UI](https://github.com/ChuniPingu/PenguinTools.UI) by Foahh. It bundles [PenguinTools Extend](https://github.com/GiftiaAIRA/PenguinTools), the PenguinTools converter with support for charts from extended Margrete releases (2.3 and later) in addition to the official editors.

企鹅工具箱 Extend 基于 Foahh 的企鹅工具箱（PenguinTools）。它在原版功能之外，支持扩展版 Margrete（2.3 及以后）的谱面。问题请在本仓库反馈，不要提交到原项目。

[下载 / Download](https://github.com/GiftiaAIRA/PenguinTools.UI/releases/latest)

The app updates itself from this repository's GitHub releases. It does not install updates from the original project.

## Prerequisites

- Git, Vite+, and Bun
- Rust with the Windows MSVC target, .NET SDK, and Visual Studio C++ build tools

Use the tool versions recorded in repository configuration. See [development setup](docs/development.md) for native build requirements.

## Quick start

```powershell
git clone --recurse-submodules https://github.com/GiftiaAIRA/PenguinTools.UI.git
cd PenguinTools.UI
vp install
vp run setup
vp run tauri:dev
```

Setup initializes submodules and links the CLI translations. The first desktop launch builds and stages the CLI runtime.

## Common commands

| Command                      | Purpose                                                 |
| ---------------------------- | ------------------------------------------------------- |
| `vp run dev`                 | Start the frontend dev server                           |
| `vp run tauri:dev`           | Build the CLI runtime and launch the desktop app        |
| `vp run stage:runtime`       | Rebuild and stage the bundled CLI                       |
| `vp run build`               | Type-check and build the frontend                       |
| `vp check` / `vp test --run` | Run frontend checks and tests                           |
| `vp run tauri:build`         | Build the Windows installer with an updater signing key |

## Documentation

- [Development, checks, and troubleshooting](docs/development.md)
- [Application architecture and runtime](docs/architecture.md)
- [Releases](docs/release.md)
- [Writing release notes](docs/changelog.md)

Licensed under the [MIT license](LICENSE).
