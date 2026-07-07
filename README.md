### Hi, I'm Huanming

Senior cross-platform engineer focused on React Native, native runtime infrastructure, performance, and reliability for high-trust consumer applications.

At [OneKey](https://onekey.so), I build core app infrastructure across iOS, Android, desktop, browser extension, and web for a multi-platform wallet supporting 80+ chains. My recent work centers on startup performance, native/background runtimes, WebView-heavy product surfaces, secure device flows, update delivery, and CI guardrails for large monorepos.

---

#### Current focus

- Cross-platform app infrastructure for React Native, Electron, native modules, and WebView-heavy clients.
- Startup and runtime performance: background runtimes, dependency graphs, first-screen budgets, and bridge traffic.
- Reliability systems for update delivery, bundle recovery, WebView lifecycle management, and release safety.
- Security-sensitive product flows around biometrics, hardware wallets, sensitive screens, and transaction controls.

#### Selected work

Three representative OneKey case studies where I owned or significantly shaped cross-platform systems:

- **Startup performance and CI guardrails.** Re-architected startup around native background runtime, bundle splitting, cold-start cache, and dependency-graph budgets. Home first-screen render improved from ~1.8s to <250ms on iPhone 17 Pro, and from ~3.5s to 600-650ms on Redmi K60 Pro; CI now blocks non-critical modules from entering startup paths. [Architecture](https://github.com/OneKeyHQ/app-monorepo/pull/10969) · [Web](https://github.com/OneKeyHQ/app-monorepo/pull/10112) · [Desktop](https://github.com/OneKeyHQ/app-monorepo/pull/12135) · [Budgets](https://github.com/OneKeyHQ/app-monorepo/pull/12281)
- **Reliability and recovery for bridge-heavy clients.** Fixed production responsiveness issues across React Native bridge traffic, token-list rendering, DApp WebViews, and OTA delivery. Work covered background-to-main batching, row-level update isolation, bounded WebView lifecycles, resumable/background downloads, and split-bundle self-healing. [Runtime](https://github.com/OneKeyHQ/app-monorepo/pull/11740) · [Rendering](https://github.com/OneKeyHQ/app-monorepo/pull/12068) · [WebView](https://github.com/OneKeyHQ/app-monorepo/pull/11854) · [Recovery](https://github.com/OneKeyHQ/app-monorepo/pull/12032)
- **Security-critical wallet and device flows.** Shipped flows where correctness and user trust matter more than feature volume: sensitive-screen protection, biometric and Windows Hello auth, biometric-change detection, transfer allowlists, and hardware-wallet onboarding. [SecureView](https://github.com/OneKeyHQ/app-monorepo/pull/4441) · [Windows Hello](https://github.com/OneKeyHQ/app-monorepo/pull/5917) · [Biometric changes](https://github.com/OneKeyHQ/app-monorepo/pull/6655)

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
