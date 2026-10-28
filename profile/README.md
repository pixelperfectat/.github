## Pixel Perfect · André Flitsch

Senior software engineer and e-commerce specialist in Austria. I build and maintain **Magento 2 / Mage-OS** extensions and the integrations around them (ERP, PIM, CRM), with a focus on code that stays upgradeable for years.

### Featured modules

| Module | What it does | Release | CI |
|---|---|---|---|
| [**module-hyva-cookie-consent**](https://github.com/pixelperfectat/module-hyva-cookie-consent) | GDPR cookie consent for Hyvä: categories, Google Consent Mode v2, consent-gated trackers that work under a strict Content Security Policy | [![Packagist](https://img.shields.io/packagist/v/pixelperfectat/module-hyva-cookie-consent)](https://packagist.org/packages/pixelperfectat/module-hyva-cookie-consent) | [![CI](https://github.com/pixelperfectat/module-hyva-cookie-consent/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/pixelperfectat/module-hyva-cookie-consent/actions/workflows/ci.yml) |
| [**magento2-module-discount-exclusion**](https://github.com/pixelperfectat/magento2-module-discount-exclusion) | Stops cart price rules from discounting products that are already reduced, with an optional per-rule top-up | [![Packagist](https://img.shields.io/packagist/v/pixelperfectat/magento2-module-discount-exclusion)](https://packagist.org/packages/pixelperfectat/magento2-module-discount-exclusion) | [![CI](https://github.com/pixelperfectat/magento2-module-discount-exclusion/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/pixelperfectat/magento2-module-discount-exclusion/actions/workflows/ci.yml) |
| [**magento2-klaviyo-hyva-compat**](https://github.com/pixelperfectat/magento2-klaviyo-hyva-compat) | Klaviyo on Hyvä storefronts: tracking, cart and customer identify, respecting Magento's cookie restriction | [![Packagist](https://img.shields.io/packagist/v/pixelperfectat/magento2-klaviyo-hyva-compat)](https://packagist.org/packages/pixelperfectat/magento2-klaviyo-hyva-compat) | [![CI](https://github.com/pixelperfectat/magento2-klaviyo-hyva-compat/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/pixelperfectat/magento2-klaviyo-hyva-compat/actions/workflows/ci.yml) |
| [**magento2-klaviyo-hyva-cookie-consent**](https://github.com/pixelperfectat/magento2-klaviyo-hyva-cookie-consent) | Loads Klaviyo only after marketing consent, checkout included | [![Packagist](https://img.shields.io/packagist/v/pixelperfectat/magento2-klaviyo-hyva-cookie-consent)](https://packagist.org/packages/pixelperfectat/magento2-klaviyo-hyva-cookie-consent) | [![CI](https://github.com/pixelperfectat/magento2-klaviyo-hyva-cookie-consent/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/pixelperfectat/magento2-klaviyo-hyva-cookie-consent/actions/workflows/ci.yml) |

### How these modules are built

Every module goes through the same gates, defined once and shared:

- **[coding-standard](https://github.com/pixelperfectat/coding-standard)**: one phpcs ruleset (Magento's plus house rules), PHPStan level 6, and checks Magento's own tooling misses, such as classes wired in XML that don't exist.
- **[ci-templates](https://github.com/pixelperfectat/ci-templates)**: one CI pipeline for GitHub and GitLab. Lint, coding standard, static analysis, unit tests and **mutation testing with Infection**, so the tests prove they would catch a bug, not just that they run.
- **Releases** follow semantic versioning with a [Keep a Changelog](https://keepachangelog.com) entry; `main` only changes through a pull request with green CI.
- **Docs say what the code does**, including known limitations, linked to issues.

### What I work on

- Magento 2 / Mage-OS and Hyvä extensions
- Integrations between shop, ERP, PIM (Akeneo) and CRM
- Import and export pipelines
- Moving legacy PHP to tested, upgradeable code
- CI/CD and automated QA for commerce teams

**Stack:** PHP 8, Magento 2 / Mage-OS, Hyvä, Symfony components, Akeneo, MySQL, OpenSearch, Docker, GitHub Actions and GitLab CI.

### Contact

[pixelperfect.at](https://pixelperfect.at)
