<div align="center">
  <img src="./Resources/clipy_logo.png" width="400">
</div>

<br>

![CI](https://github.com/xgitqa/Clipy-apple-silicon/workflows/CI/badge.svg)

Clipy is a Clipboard extension app for macOS — **Apple Silicon only** (arm64). No Rosetta 2 required.

---

__Requirement__: Mac with Apple Silicon (M1 or later), macOS 13 Ventura or later

> **Note:** This fork removes Intel (x86\_64) support. Apple is ending Rosetta 2 support in a future macOS release. This build targets arm64 natively and does not run on Intel Macs.

__Distribution Site__ : <https://clipy-app.com>

<img src="http://clipy-app.com/img/screenshot1.png" width="400">

### Development Environment
* macOS 26 Tahoe
* Xcode 26.5

### How to Build
macOS checks Accessibility permission by the app's code signature. If Clipy is built without a stable signing certificate, macOS may ask for Accessibility permission again for every build.

For this reason, the default signing settings use the Clipy signing certificate. This certificate is available only to the maintainer, so local builds require switching to ad-hoc signing before building.

#### Build for ad-hoc usage

1. Open `Clipy.xcodeproj` in Xcode.
2. Switch to ad-hoc build mode:
    1. Open `Configurations/CodeSigning.xcconfig`.
    2. Uncomment `#include "Configurations/CodeSigning-AdHoc.xcconfig"`.
3. Build the `Clipy` scheme.

### Localization Contributors
Clipy is looking for localization contributors.  
If you can contribute, please see [CONTRIBUTING.md](https://github.com/Clipy/Clipy/blob/master/.github/CONTRIBUTING.md)

### Distribution
If you distribute derived work, especially in the Mac App Store, I ask you to follow two rules:

1. Don't use `Clipy` and `ClipMenu` as your product name.
2. Follow the MIT license terms.

Thank you for your cooperation.

### Backers

Support us with a monthly donation and help us continue our activities. [[Become a backer](https://opencollective.com/clipy#backer)]

<a href="https://opencollective.com/clipy#backers"><img src="https://opencollective.com/clipy/backers.svg?avatarHeight=36&width=600" /></a>

### Sponsors

Become a sponsor and get your logo on our README on Github with a link to your site. [[Become a sponsor](https://opencollective.com/clipy#sponsor)]

<a href="https://opencollective.com/clipy#sponsors"><img src="https://opencollective.com/clipy/sponsors.svg?avatarHeight=36&width=600" /></a>

### Licence
Clipy is available under the MIT license. See the LICENSE file for more info.

Icons are copyrighted by their respective authors.

### Special Thanks
__Thank you for [@naotaka](https://github.com/naotaka) who have published [ClipMenu](https://github.com/naotaka/ClipMenu) as OSS.__
