# Threecommerce_AdminUserTimeZone: per-user time zone for the Magento 2 admin

Team in different countries? Everybody sees the admin in their own time. Magento 2 uses a single time zone, the one configured for the store. This module adds a Timezone field to the admin user and applies it to the whole backend while that user is logged in.

**Compatibility:** Magento Open Source / Adobe Commerce 2.4.4 – 2.4.9 · Mage-OS 1.x / 3.x · PHP 8.1 – 8.4 · Any frontend theme (admin-only)
**License:** free · **Current version:** see [Releases](../../releases)

## Features

- Adds a **Timezone** select to the admin user (System → Permissions → All Users) with every available time zone.
- Dates in the admin are shown in the time zone of the logged-in user.
- With "Use Default" the store time zone applies, as usual.
- The storefront is not touched: the store keeps using its standard configuration.

## Requirements

- Magento Open Source / Adobe Commerce 2.4.4+ or Mage-OS
- PHP 8.1 – 8.4
- Native modules: `Magento_User`, `Magento_Backend`
- Package: `threecommerce/m2-base` (installed automatically by Composer)

## Installation

The package is distributed through our Composer repository at `repo.threecommerce.it`. Request the credentials from the [product page](https://www.threecommerce.it/fuso-orario-per-utente-admin-magento-2?utm_source=github&utm_medium=readme&utm_campaign=magento2-admin-user-timezone), then:

```bash
composer config repositories.threecommerce composer https://repo.threecommerce.it
composer require threecommerce/m2-admin-user-time-zone
bin/magento module:enable Threecommerce_AdminUserTimeZone
bin/magento setup:upgrade
bin/magento cache:flush
```

## Configuration

Admin → **System → Permissions → All Users** → open the user → **Timezone**.

## Documentation and support

- Product page: [threecommerce.it/fuso-orario-per-utente-admin-magento-2](https://www.threecommerce.it/fuso-orario-per-utente-admin-magento-2?utm_source=github&utm_medium=readme&utm_campaign=magento2-admin-user-timezone)
- [Changelog](CHANGELOG.md) (in Italian)
- Support and custom development: [threecommerce.it/contatti](https://www.threecommerce.it/contatti?utm_source=github&utm_medium=readme&utm_campaign=magento2-admin-user-timezone)

---

*This repository is the public showcase of the module. The source code is kept in a private repository.*
