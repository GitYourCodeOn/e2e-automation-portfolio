# E2E test automation portfolio

Public test frameworks by [GitYourCodeOn](https://github.com/GitYourCodeOn). Each repository is clone-and-run, with GitHub Actions where the target site or API is still live.

This is the page to share on a CV. GitHub does not group repositories into folders, so this README is the index.

## UI end-to-end

| Repository | Stack | Target |
| --- | --- | --- |
| [DemoAutomation](https://github.com/GitYourCodeOn/DemoAutomation) | C#, Reqnroll (BDD), NUnit, Selenium 4, page objects | [Automation Exercise](https://www.automationexercise.com/) shop: account, basket, category, search, contact |
| [playwright-shop-tests](https://github.com/GitYourCodeOn/playwright-shop-tests) | Playwright TypeScript (fluent API) and Playwright C# (UI) | Same shop journeys over API and UI: products, search, account |
| [cypress_typescript](https://github.com/GitYourCodeOn/cypress_typescript) | Cypress, TypeScript, Cucumber | DuckDuckGo search |
| [WebdriverIO](https://github.com/GitYourCodeOn/WebdriverIO) | WebdriverIO, Mocha | Sauce Demo login and checkout |
| [C-Selenium](https://github.com/GitYourCodeOn/C-Selenium) | Archive of the original Selenium 3 / SpecFlow suite | Replaced by DemoAutomation |

## API and performance

| Repository | Stack | Target |
| --- | --- | --- |
| [Docker-E2e](https://github.com/GitYourCodeOn/Docker-E2e) | Cypress, Cucumber, Docker | Public users API: create, list, get, 404 |
| [api-performance-gatling](https://github.com/GitYourCodeOn/api-performance-gatling) | Gatling, Maven, Docker | Load test against the same public users API |
| [CovidRatesAPICheck](https://github.com/GitYourCodeOn/CovidRatesAPICheck) | C#, SpecFlow | COVID statistics APIs |

## Take-home tasks

Public demos rewritten without company names. Suites that still hit private training apps or contain product-specific credentials stay private and are not listed.

| Repository | Stack | Target |
| --- | --- | --- |
| [wdio-typescript-login-demo](https://github.com/GitYourCodeOn/wdio-typescript-login-demo) | WebdriverIO 9, TypeScript, Mocha, page objects | [The Internet](https://the-internet.herokuapp.com/) login (valid + invalid) |

## Mobile e2e

| Repository | Stack | Notes |
| --- | --- | --- |
| [detox-mobile-pom](https://github.com/GitYourCodeOn/detox-mobile-pom) | Detox, TypeScript, page objects | Structure template: Matchers / Gestures / Assertions + POM. CI typechecks; no app binary to build. |

### Mobile e2e open source projects

Contributions to [MetaMask Mobile](https://github.com/MetaMask/metamask-mobile) under [Andepande](https://github.com/Andepande) — Detox-era e2e, API mocking, CI parallelism, and reliability work. The repo has since moved primary smoke coverage toward Appium; the commits below show the Detox and platform work shipped on `main`.

Selected commits:

- [E2E Mocking Setup For Detox Tests](https://github.com/MetaMask/metamask-mobile/commit/2cf43036e96778d1b5a91d01937c984f8a696f11) — Detox API mocking foundation
- [Refining E2E Testing with API Mocking](https://github.com/MetaMask/metamask-mobile/commit/f36d6c91df21ba5a397c94af864122ed5a041b1d) — Mocking refinements for stable e2e
- [Parallel execution support for Android in Bitrise CI](https://github.com/MetaMask/metamask-mobile/commit/dd025c1cfd6f6b409ba34da8b4277239a8fa2e62) — Split smoke across VMs
- [Screenshots on failure implementation](https://github.com/MetaMask/metamask-mobile/commit/c068e9cefe9cdb31887550a1712eab7aea7ea8b9) — Failure artefacts for Detox runs
- [Removing test selector strings within app code](https://github.com/MetaMask/metamask-mobile/commit/89eb8cd63db54ea2ba0efffe948a026989e99aef) — Cleaner testID / selector separation
- [e2e test coverage for solana](https://github.com/MetaMask/metamask-mobile/commit/afd777011c4ca732c3fb6992c56e3d8be4dd72a8) / [snap mobile e2e implementation](https://github.com/MetaMask/metamask-mobile/commit/91a8ce082e25be5e64cd9bb6bb3dcf14caebcaca) — Feature coverage
- [Enable e2e testing for flask builds in CI](https://github.com/MetaMask/metamask-mobile/commit/72e749119b6e255cbddf15c919ac4fc5d8e99b58) — Flask smoke in pipeline

Full history: [commits by Andepande](https://github.com/MetaMask/metamask-mobile/commits/main/?author=Andepande).

## How to review

1. Open **DemoAutomation** for a full BDD UI framework (the Azure DevOps project copied here).
2. Open **playwright-shop-tests** for fluent Playwright API tests next to the same journeys in Playwright C#.
3. Open **Docker-E2e** for API testing in Cypress, including a Dockerfile.
4. Open **api-performance-gatling** for Gatling performance tests.
5. Open **detox-mobile-pom** for mobile Detox + TypeScript page-object structure.
6. Open **wdio-typescript-login-demo** for a take-home style WDIO + TypeScript login suite.
