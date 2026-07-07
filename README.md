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

Recent OneKey work where I owned or significantly shaped cross-platform systems:

- **Cut startup time across mobile, web, and desktop.** Led startup architecture across [native background runtime, bundle splitting, and cold-start cache](https://github.com/OneKeyHQ/app-monorepo/pull/10969), then extended the same discipline to [web cold startup](https://github.com/OneKeyHQ/app-monorepo/pull/10112), [desktop startup](https://github.com/OneKeyHQ/app-monorepo/pull/12135), and [startup path trimming](https://github.com/OneKeyHQ/app-monorepo/pull/12130). In release builds measured on the same devices, Home first-screen render improved from ~1.8s to <250ms on iPhone 17 Pro, and from ~3.5s to 600-650ms on Redmi K60 Pro.
- **Built CI guardrails for startup and monorepo quality.** Turned first-screen dependency graphs into budgeted CI gates with [startup graph budgets](https://github.com/OneKeyHQ/app-monorepo/pull/12281) and [native/web graph tightening](https://github.com/OneKeyHQ/app-monorepo/pull/12286), catching non-critical modules before they enter startup paths. Extended the same guardrail model to module boundaries, import rules, QA test IDs, and [AI-assisted UI regression checks](https://github.com/OneKeyHQ/app-monorepo/pull/11963).
- **Improved responsiveness in bridge-heavy React Native surfaces.** Fixed production tab-switch freezes caused by [background-to-main bridge storms](https://github.com/OneKeyHQ/app-monorepo/pull/11740), isolated [token-list row updates](https://github.com/OneKeyHQ/app-monorepo/pull/12068) so live price ticks update changed rows instead of whole lists, and hardened WebView-heavy surfaces with [bounded DApp browser lifecycles](https://github.com/OneKeyHQ/app-monorepo/pull/11854) and warm TradingView charts.
- **Hardened update delivery and bundle recovery infrastructure.** Built [resumable app updates](https://github.com/OneKeyHQ/app-monorepo/pull/11535), [multi-range/background downloads](https://github.com/OneKeyHQ/app-monorepo/pull/11872), [split-bundle self-healing](https://github.com/OneKeyHQ/app-monorepo/pull/12032), and native downloader modules so OTA bundles and release delivery recover more reliably across platforms.
- **Shipped security-critical wallet and device flows.** Built sensitive-screen protection with [SecureView](https://github.com/OneKeyHQ/app-monorepo/pull/4441), biometric and [Windows Hello](https://github.com/OneKeyHQ/app-monorepo/pull/5917) flows, [biometric-change detection](https://github.com/OneKeyHQ/app-monorepo/pull/6655), transfer allowlists, and hardware-wallet onboarding for signing, recovery, and device connection workflows.

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
