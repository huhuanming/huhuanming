### Hi, I'm Huanming

Core developer at [OneKey](https://onekey.so), building open-source crypto wallet software across mobile, desktop, extension, and web.

I mostly work around React Native, native platform bridges, wallet security, performance, and reliability for multi-chain products.

---

#### Current focus

- Leading development of [OneKey App](https://github.com/OneKeyHQ/app-monorepo), a multi-platform wallet supporting 80+ chains.
- Building React Native and native modules for iOS, Android, desktop, and WebView-heavy product surfaces.
- Improving security-sensitive wallet flows, including hardware wallets, air-gapped usage, biometric authentication, and DApp browser reliability.

#### Selected work

- [OneKey App](https://github.com/OneKeyHQ/app-monorepo): cross-platform wallet application architecture, product delivery, and day-to-day engineering.
- [OneKey native modules](https://github.com/OneKeyHQ/app-modules): native capabilities for React Native wallet features.
- Performance highlights:
  - [Mobile startup architecture](https://github.com/OneKeyHQ/app-monorepo/pull/10969): native background runtime, three-bundle split, cold-start SSR cache, and CI startup guards; by July 2026, Home first-screen render hit <250ms on iPhone 17 Pro and 600-650ms on Redmi K60 Pro, down from earlier 2026 baselines of ~2.8s on Android and ~550ms on iPhone 17 Pro.
  - [Web cold startup](https://github.com/OneKeyHQ/app-monorepo/pull/10112): reduced black-screen time from ~5.1s to ~1.3s with batched IndexedDB reads and render stabilization.
  - [Desktop cold startup](https://github.com/OneKeyHQ/app-monorepo/pull/12135): slimmed the Electron main bundle from 25.4MB to 5.8MB and cut first-line startup from 647ms to 344ms.
  - [Startup path optimization](https://github.com/OneKeyHQ/app-monorepo/pull/12130): lazy-loaded per-chain dapp providers, Lottie, and lodash-heavy paths so first paint avoids non-critical startup work.
  - [Runtime responsiveness](https://github.com/OneKeyHQ/app-monorepo/pull/11740): batched bg -> main atom broadcasts and token merge bridge calls to fix production tab-switch freezes.
  - [Token list rendering](https://github.com/OneKeyHQ/app-monorepo/pull/12068): moved derivation to the background runtime and changed price ticks from O(all tokens) to O(changed rows).

#### Open source

- [DefinitelyTyped](https://github.com/DefinitelyTyped/DefinitelyTyped): 20+ merged PRs for React Native and TypeScript definitions, including
  [fetchBundle](https://github.com/DefinitelyTyped/DefinitelyTyped/pull/22023),
  [MaskedView](https://github.com/DefinitelyTyped/DefinitelyTyped/pull/19522), and
  [timer typings](https://github.com/DefinitelyTyped/DefinitelyTyped/pull/19809).
- React Native ecosystem contributions and maintenance work across wallet, WebView, navigation, native module, and build tooling surfaces.
- [qiniu_upload](https://github.com/huhuanming/qiniu_upload): Objective-C SDK for batch Qiniu uploads, MIT licensed and used by older iOS/macOS projects.

#### Tech stack

```text
Frontend        React Native · React · TypeScript · Electron
Native          iOS · Android · Swift · Objective-C · Kotlin
Wallet          Multi-chain · Hardware Wallets · Air-gapped Security · WebView
Engineering     Monorepo · Native Modules · CI/CD · Performance
```

#### GitHub stats

<p>
  <img height="160" src="https://github-readme-stats.vercel.app/api?username=huhuanming&show_icons=true&theme=default&hide_border=true&count_private=true" />
  <img height="160" src="https://github-readme-stats.vercel.app/api/top-langs/?username=huhuanming&layout=compact&theme=default&hide_border=true" />
</p>

#### Connect

<a href="https://github.com/huhuanming">
  <img src="https://img.shields.io/badge/-GitHub-181717?style=flat&logo=github" />
</a>
<a href="https://onekey.so">
  <img src="https://img.shields.io/badge/-OneKey-00DC82?style=flat&logoColor=white" />
</a>

---

<p align="center">
  <i>Crypto security in my head: air-gapped on top, hot wallets on sides.</i>
</p>
