# Pavel Zhukov Atum

Senior SDET: I build test automation for web applications and APIs, and fix test suites that teams stopped trusting.

| Project | What it shows | Published results |
| --- | --- | --- |
| [Toolshop-Test-Automation-Framework](https://github.com/WolfGung/Toolshop-Test-Automation-Framework) | A test automation framework built from scratch for an online shop, with test design documents | [Allure report](https://wolfgung.github.io/Toolshop-Test-Automation-Framework/) |
| [Marketplace-Test-Automation-Framework](https://github.com/WolfGung/Marketplace-Test-Automation-Framework) | API and browser tests in CI against a copy of a public demo shop kept in the repository, with a nightly check that the copy still matches the original | [Allure report](https://wolfgung.github.io/Marketplace-Test-Automation-Framework/) |
| [Web-Scraping-Automation-Framework](https://github.com/WolfGung/Web-Scraping-Automation-Framework) | A nightly scraper of three sources that reports what changed and publishes the data | [Data and report](https://wolfgung.github.io/Web-Scraping-Automation-Framework/) |
| [Test-Suite-Rescue](https://github.com/WolfGung/Test-Suite-Rescue) | A flaky, slow test suite cured without losing coverage, with twenty measured runs of each version | [Measurements](https://github.com/WolfGung/Test-Suite-Rescue#readme) |
| [API-Test-Generator](https://github.com/WolfGung/API-Test-Generator) | A command-line tool that turns an OpenAPI document or a Postman collection into a runnable pytest suite | [Generated suites](https://github.com/WolfGung/API-Test-Generator/tree/main/examples) |
| [Accessibility-Test-Automation-Framework](https://github.com/WolfGung/Accessibility-Test-Automation-Framework) | An axe-core scan and keyboard-only checks against a shop in an accessible and a deliberately broken mode, every finding mapped to a WCAG criterion | [Findings and report](https://wolfgung.github.io/Accessibility-Test-Automation-Framework/) |
| [LLM-Evaluation-Framework](https://github.com/WolfGung/LLM-Evaluation-Framework) | A RAG support assistant and ticket triage evaluated in layers, with an LLM judge measured against human labels and a regression gate in CI | [Results and report](https://wolfgung.github.io/LLM-Evaluation-Framework/) |
| [Load-Testing-Automation-Framework](https://github.com/WolfGung/Load-Testing-Automation-Framework) | Python and Locust API load tests that identify a catalogue bottleneck and measure its repair under the same workload | [Measurements and report](https://wolfgung.github.io/Load-Testing-Automation-Framework/) |

- **Test automation from scratch:** API, browser and end-to-end suites that run in CI on every push.
- **Fixing what already exists:** flaky tests, slow runs, and suites that need a restart between runs.
- **Data work:** scrapers and scheduled monitoring with exports to CSV and JSON.
- **Accessibility testing:** an axe-core scan and keyboard-only checks in CI, findings mapped to WCAG 2.1 AA criteria, and a manual checklist for what automation cannot see.
- **API suites from the documents you already have:** an OpenAPI document or a Postman collection turned into a pytest suite that runs in CI.
- **Testing AI features:** a chatbot or RAG assistant evaluated in CI with rules, reference checks, prompt-injection and data-leak cases, repeat-run stability, and an LLM judge measured against human labels.
- **Load and performance testing:** API business flows under load, stress, spike and soak workloads, bottleneck diagnosis, measured repairs, and repeatable performance checks.

## Stack

Python, pytest, Playwright, Selenium, httpx, Locust, API load testing, REST API testing, OpenAPI, Postman, axe-core, WCAG 2.1, LLM evaluation (RAG, LLM-as-a-judge), OpenRouter, Pydantic, SQLAlchemy, FastAPI, Docker, GitHub Actions, GitLab CI, Allure.

Seven years in test automation, mostly in FinTech and payments, e-commerce and marketplaces, cybersecurity, and telecom and VoIP products.

## Selected work

Each repository publishes test results or measured evidence, so every number in its README can be checked.

**[Toolshop-Test-Automation-Framework](https://github.com/WolfGung/Toolshop-Test-Automation-Framework)** — a test framework built from scratch for an online shop: API, browser and end-to-end cases against a public demo shop or a local Docker stand of the same application, with test design documents, page objects and an Allure report on GitHub Pages. Shows the full cycle from requirements analysis to a suite that runs in CI.

**[Marketplace-Test-Automation-Framework](https://github.com/WolfGung/Marketplace-Test-Automation-Framework)** — API and browser tests for a marketplace shop, run against a small stand shipped in the repository, with a smoke set, a video and a Playwright trace of each end-to-end test, and a published Allure report with a trend across runs. Shows an API test suite and end-to-end tests for a checkout flow kept honest by CI.

**[Web-Scraping-Automation-Framework](https://github.com/WolfGung/Web-Scraping-Automation-Framework)** — a scraper that collects two practice sites and a demo store of its own, over HTTP and through a browser, detects changes between nightly runs and publishes the data, the change report, a recording and the test report to GitHub Pages. Shows polite scraping (rate limits, retries, robots.txt), data extraction to CSV and JSON, and scheduled monitoring.

**[Test-Suite-Rescue](https://github.com/WolfGung/Test-Suite-Rescue)** — a deliberately sick test suite and its cured version with the same checks, on Playwright and on Selenium, and the measured difference: twenty runs of each against the same application, reproducible with one command, with a diagnosis of each disease. Shows what fixing flaky tests and reducing run time looks like when it is done, not described.

**[API-Test-Generator](https://github.com/WolfGung/API-Test-Generator)** — a command-line tool that reads an OpenAPI 3 document or a Postman collection into one model and writes a pytest suite from it: a positive test per operation, a negative test per required parameter and field, a check without credentials, and response validation against generated Pydantic models. Four generated suites are committed and reproduced byte for byte in CI, and the two built from a sample API run against it on every push. Shows how a first API suite for an existing backend is produced from the documents a team already has.

**[Accessibility-Test-Automation-Framework](https://github.com/WolfGung/Accessibility-Test-Automation-Framework)** — an axe-core scan and keyboard-only checks against a small shop served in an accessible mode and in a mode with ten planted WCAG 2.1 AA violations, run in both modes on every push: the scan must find what it can, the keyboard checks the rest, and each violation's detection is established by the tests, not asserted. What neither layer can see goes to a manual checklist. Shows accessibility checks wired into CI with findings mapped to criteria, and honest limits.

**[LLM-Evaluation-Framework](https://github.com/WolfGung/LLM-Evaluation-Framework)** — a support assistant over a small knowledge base and a ticket triage feature, each with two prompt versions, evaluated in layers from cheap to expensive: deterministic rules, reference facts and labels, safety cases against prompt injection and data leaks, repeat-run stability, and an LLM judge that is measured itself, against blind human labels and for position bias with swapped pairs. A real recording of 706 calls to free models replays in CI, so every run is free and a regression gate fails the build when a prompt or model change makes things worse. Shows how to evaluate LLM features and when an LLM judge can be trusted.

**[Load-Testing-Automation-Framework](https://github.com/WolfGung/Load-Testing-Automation-Framework)** — Python and Locust tests against a local FastAPI shop: browsing and checkout with isolated sessions and carts, response validation, and smoke, load, stress, spike and soak profiles. A measured comparison diagnoses downstream pool contention in the catalogue and checks a batching repair under the same workload. The published report includes per-operation percentiles, throughput, errors, resource charts and raw CSV evidence; configurable thresholds provide a repeatable performance gate. Shows how to find an API bottleneck, measure its repair and hand over tests and evidence a client can reproduce.

## Available for freelance work

Short, well-defined jobs: a test automation framework from scratch, an API test suite for an existing backend (from its OpenAPI document or Postman collection), end-to-end tests for a critical flow, API load and performance testing with bottleneck diagnosis, accessibility testing against WCAG 2.1 AA, testing LLM features such as chatbots and RAG assistants, fixing flaky tests and reducing run time, setting up CI for existing tests, scrapers and data pipelines.

I use AI coding assistants (Claude Code, Codex) to move faster. Design decisions, test design and code review stay with me, and every change ships with tests. With your code and data I follow your policy: if AI tools are not allowed on your project, I don't use them.

Guru profile: https://www.guru.com/freelancers/pavel-zhukov-atum

Time zone: Central European Time (CET/CEST), so my working hours overlap with Central European business hours. I work in writing — a clear task description and a repository link are enough to start.
