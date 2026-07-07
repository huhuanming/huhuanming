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

Recent OneKey work where I owned or significantly shaped cross-platform systems:

- **Startup performance across mobile, web, and desktop:** [Metro code splitting](https://github.com/OneKeyHQ/app-monorepo/pull/3922), [launch-time monitoring](https://github.com/OneKeyHQ/app-monorepo/pull/8585), and [startup analysis tooling](https://github.com/OneKeyHQ/app-monorepo/pull/8675) established the measurement loop; [Mobile startup architecture](https://github.com/OneKeyHQ/app-monorepo/pull/10969) then introduced native background runtime, three-bundle split, and cold-start SSR cache. In release builds measured on the same devices, Home first-screen render improved from ~1.8s to <250ms on iPhone 17 Pro, and from ~3.5s to 600-650ms on Redmi K60 Pro. [Web cold startup](https://github.com/OneKeyHQ/app-monorepo/pull/10112), [desktop cold startup](https://github.com/OneKeyHQ/app-monorepo/pull/12135), and [startup path trimming](https://github.com/OneKeyHQ/app-monorepo/pull/12130) expanded the same discipline across web, Electron, and native first-screen paths.
- **Startup CI guardrails and monorepo quality gates:** [startup graph budgets](https://github.com/OneKeyHQ/app-monorepo/pull/12281) and [native/web graph tightening](https://github.com/OneKeyHQ/app-monorepo/pull/12286) turn first-screen dependency graphs into CI gates, catching non-critical modules before they enter startup paths. [Folder/language/import linting](https://github.com/OneKeyHQ/app-monorepo/pull/4038), [module-boundary checks](https://github.com/OneKeyHQ/app-monorepo/pull/6539), [QA testID coverage](https://github.com/OneKeyHQ/app-monorepo/pull/10966), and an [AI-agent UI regression runner](https://github.com/OneKeyHQ/app-monorepo/pull/11963) extend that guardrail mindset across a large AI-assisted monorepo.
- **Runtime responsiveness and list rendering:** [bg -> main batching](https://github.com/OneKeyHQ/app-monorepo/pull/11740) fixed production tab-switch freezes caused by bridge storms, while [token-list cell isolation](https://github.com/OneKeyHQ/app-monorepo/pull/12068) moved derivation to the background runtime so price ticks update changed rows instead of whole lists.
- **Update delivery and bundle recovery infrastructure:** [resumable AppUpdate](https://github.com/OneKeyHQ/app-monorepo/pull/11535), [multi-range/background downloads](https://github.com/OneKeyHQ/app-monorepo/pull/11872), [OCDS v1.1 orchestration](https://github.com/OneKeyHQ/app-monorepo/pull/12121), [split-bundle route self-healing](https://github.com/OneKeyHQ/app-monorepo/pull/12032), native [Nitro downloader modules](https://github.com/OneKeyHQ/app-modules/pull/60), [kill->restart resume hardening](https://github.com/OneKeyHQ/app-modules/pull/66), and an [OCDS v1.1 concurrent downloader standard](https://github.com/OneKeyHQ/app-modules/pull/70) harden hot updates, OTA bundles, and cross-platform release delivery.
- **DApp browser and trading WebView platform:** [DApp browser WebView LRU](https://github.com/OneKeyHQ/app-monorepo/pull/11854) bounds live WebView memory, while [chart WebView bridge work](https://github.com/OneKeyHQ/app-modules/pull/77), [offline/warm TradingView charts](https://github.com/OneKeyHQ/app-monorepo/pull/11922), [runtime data-source switching](https://github.com/OneKeyHQ/tradingview-charting-library/pull/162), and [packaged chart distribution](https://github.com/OneKeyHQ/tradingview-charting-library/pull/164) make chart-heavy product surfaces faster and more reliable.
- **Wallet security and device flows:** [SecureView](https://github.com/OneKeyHQ/app-monorepo/pull/4441), [Windows Hello](https://github.com/OneKeyHQ/app-monorepo/pull/5917), [biometric-change detection](https://github.com/OneKeyHQ/app-monorepo/pull/6655), [transfer allowlists](https://github.com/OneKeyHQ/app-monorepo/pull/6497), and [hardware-wallet onboarding](https://github.com/OneKeyHQ/app-monorepo/pull/8869) cover signing, recovery, device connection, and sensitive-screen reliability.

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
