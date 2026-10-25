# Awesome MV3 [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of awesome resources for building Chrome, Edge, and Firefox extensions on **Manifest V3 (MV3)** — boilerplates, build tools, live reload, typed APIs, message passing, and more.

Manifest V3 is the current extension format for Chromium-based browsers
(and now Firefox). This list focuses on **MV3-ready** tools and libraries —
nothing built around `chrome.extension`, persistent background pages, or
other MV2-only patterns. Older resources are listed only when they remain
the canonical answer for an MV3 task.

## Contents

- [Boilerplates and starters](#boilerplates-and-starters)
- [Build tools and live reload](#build-tools-and-live-reload)
- [Type definitions](#type-definitions)
- [Message passing](#message-passing)
- [Storage](#storage)
- [Service Worker utilities](#service-worker-utilities)
- [Content scripts](#content-scripts)
- [UI frameworks](#ui-frameworks)
- [Testing](#testing)
- [Publishing and signing](#publishing-and-signing)
- [Side Panel API](#side-panel-api)
- [Declarative Net Request](#declarative-net-request)
- [Frameworks](#frameworks)
- [Resources](#resources)
- [Related lists](#related-lists)

## Boilerplates and starters

- [chrome-extension-vite-react](https://github.com/graybearo/chrome-extension-vite-react) - MV3 starter using Vite, React, TypeScript, with HMR and typed messaging.
- [chrome-extension-webpack-react](https://github.com/graybearo/chrome-extension-webpack-react) - MV3 starter using Webpack 5, React, TypeScript, with live reload.
- [create-chrome-ext](https://github.com/guocaoyi/create-chrome-ext) - Scaffolder for Vite-based Chrome extensions with multiple framework choices.
- [extension.js](https://github.com/extension-js/extension.js) - Build tool that creates extensions with zero configuration.
- [vitesse-webext](https://github.com/antfu/vitesse-webext) - Vite + Vue + WebExtension starter by antfu.

## Build tools and live reload

- [@crxjs/vite-plugin](https://github.com/crxjs/chrome-extension-tools) - Vite plugin that uses the manifest as the source of truth and provides HMR for popup, options, and content scripts.
- [Parcel](https://parceljs.org) - Bundler with built-in support for browser extensions.
- [webpack-ext-reloader-next](https://github.com/graybearo/webpack-ext-reloader-next) - Webpack 5 plugin for MV3 extension live reload.

## Type definitions

- [@types/chrome](https://www.npmjs.com/package/@types/chrome) - TypeScript types for the `chrome.*` APIs.
- [webextension-polyfill](https://github.com/mozilla/webextension-polyfill) - Mozilla's `browser.*` Promise-based polyfill for cross-browser parity.
- [webextension-polyfill-ts](https://github.com/lusito/webextension-polyfill-ts) - TypeScript types for `webextension-polyfill`.

## Message passing

- [mv3-message-router](https://github.com/graybearo/mv3-message-router) - Type-safe wrapper over `chrome.runtime.sendMessage` for popup, content, and SW.
- [webext-bridge](https://github.com/zikaari/webext-bridge) - Message-passing library for WebExtensions with cross-context API.
- [webext-redux](https://github.com/tshaddix/webext-redux) - Use a Redux store across content scripts, popups, and background.

## Storage

- [@webext-core/storage](https://webext-core.aklinker1.io/storage/) - Type-safe wrapper around `browser.storage` with reactivity.
- [webext-options-sync](https://github.com/fregante/webext-options-sync) - Synced options storage with defaults and migrations.

## Service Worker utilities

- [mv3-keepalive](https://github.com/graybearo/mv3-keepalive) - Keep MV3 service workers alive during async work; durable `chrome.alarms`.

## Content scripts

- [content-scripts-register-polyfill](https://github.com/fregante/content-scripts-register-polyfill) - Polyfill for `chrome.scripting.registerContentScripts`.
- [mv3-content-bridge](https://github.com/graybearo/mv3-content-bridge) - Type-safe content-script ↔ page-context bridge over `window.postMessage`.
- [@webext-core/proxy-service](https://webext-core.aklinker1.io/proxy-service/) - Type-safe RPC from content scripts to background.

## UI frameworks

- [Chakra UI](https://chakra-ui.com) - Component library with first-class support inside extensions.
- [shadcn/ui](https://ui.shadcn.com) - Copy-paste components that work well in popup and options pages.

## Testing

- [Playwright](https://playwright.dev) - Cross-browser automation with extension loading support.
- [Puppeteer](https://pptr.dev) - Headless Chromium automation; supports loading unpacked extensions.

## Publishing and signing

- [chrome-webstore-upload](https://github.com/fregante/chrome-webstore-upload) - Programmatic upload to the Chrome Web Store.
- [semantic-release-chrome](https://github.com/Roms1383/semantic-release-chrome) - Publish releases to the Chrome Web Store from CI.
- [web-ext](https://github.com/mozilla/web-ext) - Mozilla's CLI for building, running, and signing extensions.

## Side Panel API

- [chrome-extension-side-panel](https://github.com/graybearo/chrome-extension-side-panel) - MV3 starter using `chrome.sidePanel`, Vite, React, and TypeScript.
- [Chrome Side Panel API docs](https://developer.chrome.com/docs/extensions/reference/api/sidePanel) - Official documentation for the Side Panel API (Chrome 114+).

## Declarative Net Request

- [Chrome DNR docs](https://developer.chrome.com/docs/extensions/reference/api/declarativeNetRequest) - Official documentation for the rule-based network interception API replacing blocking webRequest.

## Frameworks

- [Plasmo](https://www.plasmo.com) - Opinionated framework for browser extensions, with file-system routing and a hosted publishing pipeline.
- [WXT](https://wxt.dev) - Next-gen browser-extension framework built on Vite.

## Resources

- [Chrome Extension Guide](https://github.com/theluckystrike/chrome-extension-guide) - Free guides on MV3 APIs, service workers, migration and publishing.
- [Chrome Extensions documentation](https://developer.chrome.com/docs/extensions) - Official Google Docs for the Chrome extension platform.
- [Manifest V3 migration guide](https://developer.chrome.com/docs/extensions/develop/migrate) - Official MV2 → MV3 migration guide.
- [MDN — Browser Extensions](https://developer.mozilla.org/en-US/docs/Mozilla/Add-ons/WebExtensions) - Mozilla's cross-browser extension docs.

## Related lists

- [Awesome WebExtensions](https://github.com/fregante/Awesome-WebExtensions) - Broader list covering both MV2 and MV3 by [@fregante](https://github.com/fregante).

## Contributing

Contributions welcome! Please read the [contribution guidelines](CONTRIBUTING.md) first, then open a pull request. Entries must be MV3-relevant and actively maintained.
