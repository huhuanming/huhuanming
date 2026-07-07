### Hi, I'm Huanming

Core developer at [OneKey](https://onekey.so), building open-source crypto wallet software across mobile, desktop, extension, and web.

I mostly work around React Native, native platform bridges, wallet security, performance, and reliability for multi-chain products.

---

#### Current focus

- Leading major app engineering work for [OneKey App](https://github.com/OneKeyHQ/app-monorepo), a multi-platform wallet supporting 80+ chains.
- Building React Native and native modules for iOS, Android, desktop, and WebView-heavy product surfaces.
- Improving wallet flows where reliability and security matter: hardware-wallet signing, air-gapped flows, biometric authentication, and DApp browser stability.
- Designing startup CI guardrails for AI-assisted development: first-screen checks, dependency-graph budgets, and regression gates.

#### Selected work

- [OneKey App](https://github.com/OneKeyHQ/app-monorepo): cross-platform app architecture, React Native/native integration, startup performance, and wallet feature delivery.
- [OneKey native modules](https://github.com/OneKeyHQ/app-modules): native capabilities for React Native wallet features.
- Startup performance:
  - [Mobile startup architecture](https://github.com/OneKeyHQ/app-monorepo/pull/10969): introduced native background runtime, three-bundle split, and cold-start SSR cache. In release builds measured on the same devices, Home first-screen render improved from ~1.8s to <250ms on iPhone 17 Pro, and from ~3.5s to 600-650ms on Redmi K60 Pro.
  - [Startup CI harnesses](https://github.com/OneKeyHQ/app-monorepo): enforced native/web first-screen dependency-graph budgets for AI-assisted development, catching non-critical modules entering startup paths before merge.
  - [Web cold startup](https://github.com/OneKeyHQ/app-monorepo/pull/10112): reduced black-screen time from ~5.1s to ~1.3s with batched IndexedDB reads and render stabilization.
  - [Desktop cold startup](https://github.com/OneKeyHQ/app-monorepo/pull/12135): slimmed the Electron main bundle from 25.4MB to 5.8MB and cut the Electron main-process startup marker from 647ms to 344ms.
  - [Startup path optimization](https://github.com/OneKeyHQ/app-monorepo/pull/12130): lazy-loaded per-chain dapp providers, Lottie, and lodash-heavy paths so first paint avoids non-critical startup work.
- Runtime performance:
  - [Runtime responsiveness](https://github.com/OneKeyHQ/app-monorepo/pull/11740): batched bg -> main atom broadcasts and token merge bridge calls to fix production tab-switch freezes.
  - [Token list rendering](https://github.com/OneKeyHQ/app-monorepo/pull/12068): moved derivation to the background runtime and changed price ticks from O(all tokens) to O(changed rows).

#### Open source

- [DefinitelyTyped](https://github.com/DefinitelyTyped/DefinitelyTyped): 20+ merged PRs for React Native and TypeScript definitions, including
  [fetchBundle](https://github.com/DefinitelyTyped/DefinitelyTyped/pull/22023),
  [MaskedView](https://github.com/DefinitelyTyped/DefinitelyTyped/pull/19522), and
  [timer typings](https://github.com/DefinitelyTyped/DefinitelyTyped/pull/19809).
- Occasional React Native ecosystem fixes across wallet, WebView, navigation, native modules, and build tooling.
- [qiniu_upload](https://github.com/huhuanming/qiniu_upload): MIT-licensed Objective-C SDK for batch Qiniu uploads.

#### Tech stack

```text
Frontend        React Native · React · TypeScript · Electron
Native          iOS · Android · Swift · Objective-C · Kotlin
Wallet          Multi-chain · Hardware Wallets · Air-gapped Security · WebView
Engineering     Monorepo · Native Modules · CI/CD · Performance Harnesses
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
