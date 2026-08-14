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

## How to review

1. Open **DemoAutomation** for a full BDD UI framework (the Azure DevOps project copied here).
2. Open **playwright-shop-tests** for fluent Playwright API tests next to the same journeys in Playwright C#.
3. Open **Docker-E2e** for API testing in Cypress, including a Dockerfile.
4. Open **api-performance-gatling** for Gatling performance tests.

Private take-home suites (Playwright / Lokalise, WebdriverIO ETH, Python Behave / Primer, Mocha / Deel) stay private and are not listed here.
