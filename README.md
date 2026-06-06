<div align="center">
  <img src="./Resources/clipy_logo.png" width="400">
</div>

<br>

![CI](https://github.com/xgitqa/Clipy-apple-silicon/workflows/CI/badge.svg)
[![Release](https://img.shields.io/github/v/release/xgitqa/Clipy-apple-silicon)](https://github.com/xgitqa/Clipy-apple-silicon/releases/latest)

Clipy is a Clipboard extension app for macOS — **Apple Silicon only** (arm64). No Rosetta 2 required.

---

__Requirement__: Mac with Apple Silicon (M1 or later), macOS 13 Ventura or later

> **Note:** This fork removes Intel (x86\_64) support. Apple is ending Rosetta 2 support in a future macOS release. This build targets arm64 natively and does not run on Intel Macs.

### Download

**[→ Download the latest release](https://github.com/xgitqa/Clipy-apple-silicon/releases/latest)**

Unzip and move `Clipy.app` to `/Applications`. On first launch, right-click → Open (the build is ad-hoc signed, not notarized).

#### Install via Homebrew

```sh
brew tap xgitqa/clipy-apple-silicon
brew install --cask clipy-apple-silicon
```

<img src="http://clipy-app.com/img/screenshot1.png" width="400">

### Development Environment
* macOS 26 Tahoe
* Xcode 26.5

### How to Build

Ad-hoc signing is the default — no Apple Developer account required.

1. Open `Clipy.xcodeproj` in Xcode.
2. Build the `Clipy` scheme.

> macOS checks Accessibility permission by code signature. Ad-hoc builds may prompt for Accessibility access again after each build. This is expected behaviour.

### Localization Contributors
Clipy is looking for localization contributors.  
If you can contribute, please see [CONTRIBUTING.md](.github/CONTRIBUTING.md)

### Distribution
If you distribute derived work, especially in the Mac App Store, please follow two rules:

1. Don't use `Clipy` and `ClipMenu` as your product name.
2. Follow the MIT license terms.

### Licence
Clipy is available under the MIT license. See the LICENSE file for more info.

Icons are copyrighted by their respective authors.

### Special Thanks
__Thank you for [@naotaka](https://github.com/naotaka) who have published [ClipMenu](https://github.com/naotaka/ClipMenu) as OSS.__

__Based on the original [Clipy](https://github.com/Clipy/Clipy) project by the Clipy Project.__
