# Pavel Zhukov Atum

Senior SDET: I build test automation for web applications and APIs, and fix test suites that teams stopped trusting.

| Project | What it shows | Published results |
| --- | --- | --- |
| [Toolshop-Test-Automation-Framework](https://github.com/WolfGung/Toolshop-Test-Automation-Framework) | A test automation framework built from scratch for an online shop, with test design documents | [Allure report](https://wolfgung.github.io/Toolshop-Test-Automation-Framework/) |
| [Marketplace-Test-Automation-Framework](https://github.com/WolfGung/Marketplace-Test-Automation-Framework) | API and browser tests against a shop shipped in the repository, with a nightly drift check of the public site | [Allure report](https://wolfgung.github.io/Marketplace-Test-Automation-Framework/) |
| [Web-Scraping-Automation-Framework](https://github.com/WolfGung/Web-Scraping-Automation-Framework) | A nightly scraper of three sources that reports what changed and publishes the data | [Data and report](https://wolfgung.github.io/Web-Scraping-Automation-Framework/) |
| [Test-Suite-Rescue](https://github.com/WolfGung/Test-Suite-Rescue) | A flaky, slow test suite cured without losing coverage, with twenty measured runs of each version | [Measurements](https://github.com/WolfGung/Test-Suite-Rescue#readme) |
| [API-Test-Generator](https://github.com/WolfGung/API-Test-Generator) | A command-line tool that turns an OpenAPI document or a Postman collection into a runnable pytest suite | [Generated suites](https://github.com/WolfGung/API-Test-Generator/tree/main/examples) |
| [Accessibility-Test-Automation-Framework](https://github.com/WolfGung/Accessibility-Test-Automation-Framework) | An axe-core scan and keyboard-only checks against a shop in an accessible and a deliberately broken mode, every finding mapped to a WCAG criterion | [Findings and report](https://wolfgung.github.io/Accessibility-Test-Automation-Framework/) |

- **Test automation from scratch:** API, browser and end-to-end suites that run in CI on every push.
- **Fixing what already exists:** flaky tests, slow runs, and suites that need a restart between runs.
- **Data work:** scrapers and scheduled monitoring with exports to CSV and JSON.
- **Accessibility testing:** an axe-core scan and keyboard-only checks in CI, findings mapped to WCAG 2.1 AA criteria, and a manual checklist for what automation cannot see.
- **API suites from the documents you already have:** an OpenAPI document or a Postman collection turned into a pytest suite that runs in CI.

## Stack

Python, pytest, Playwright, Selenium, httpx, REST API testing, OpenAPI, Postman, axe-core, WCAG 2.1, Pydantic, SQLAlchemy, FastAPI, Docker, GitHub Actions, GitLab CI, Allure.

Seven years in test automation, mostly in FinTech and payments, e-commerce and marketplaces, cybersecurity, and telecom and VoIP products.

## Selected work

Each repository publishes its results from its own CI run, so every number in its README can be checked.

**[Toolshop-Test-Automation-Framework](https://github.com/WolfGung/Toolshop-Test-Automation-Framework)** — a test framework built from scratch for an online shop: API, browser and end-to-end cases against a public demo shop or a local Docker stand of the same application, with test design documents, page objects and an Allure report on GitHub Pages. Shows the full cycle from requirements analysis to a suite that runs in CI.

**[Marketplace-Test-Automation-Framework](https://github.com/WolfGung/Marketplace-Test-Automation-Framework)** — API and browser tests for a marketplace shop, run against a small stand shipped in the repository, with a smoke set, video and traces for every browser test, and a published Allure report with a trend across runs. Shows an API test suite and end-to-end tests for a checkout flow kept honest by CI.

**[Web-Scraping-Automation-Framework](https://github.com/WolfGung/Web-Scraping-Automation-Framework)** — a scraper that collects two practice sites and a demo store of its own, over HTTP and through a browser, detects changes between nightly runs and publishes the data, the change report, a recording and the test report to GitHub Pages. Shows polite scraping (rate limits, retries, robots.txt), data extraction to CSV and JSON, and scheduled monitoring.

**[Test-Suite-Rescue](https://github.com/WolfGung/Test-Suite-Rescue)** — a deliberately sick test suite and its cured version with the same checks, on Playwright and on Selenium, and the measured difference: twenty runs of each against the same application, reproducible with one command, with a diagnosis of each disease. Shows what fixing flaky tests and reducing run time looks like when it is done, not described.

**[API-Test-Generator](https://github.com/WolfGung/API-Test-Generator)** — a command-line tool that reads an OpenAPI 3 document or a Postman collection into one model and writes a pytest suite from it: a positive test per operation, a negative test per required parameter and field, a check without credentials, and response validation against generated Pydantic models. Four generated suites are committed and reproduced byte for byte in CI, and the two built from a sample API run against it on every push. Shows how a first API suite for an existing backend is produced from the documents a team already has.

**[Accessibility-Test-Automation-Framework](https://github.com/WolfGung/Accessibility-Test-Automation-Framework)** — an axe-core scan and keyboard-only checks against a small shop served in an accessible mode and in a mode with ten planted WCAG 2.1 AA violations, run in both modes on every push: the scan must find what it can, the keyboard checks the rest, and each violation's detection is established by the tests, not asserted. What neither layer can see goes to a manual checklist. Shows accessibility checks wired into CI with findings mapped to criteria, and honest limits.

## Available for freelance work

Short, well-defined jobs: a test automation framework from scratch, an API test suite for an existing backend (from its OpenAPI document or Postman collection), end-to-end tests for a critical flow, accessibility testing against WCAG 2.1 AA, fixing flaky tests and reducing run time, setting up CI for existing tests, scrapers and data pipelines.

Guru profile: https://www.guru.com/freelancers/pavel-zhukov-atum

Time zone: Central European Time (CET/CEST), so my working hours overlap with Central European business hours. I work in writing — a clear task description and a repository link are enough to start.
