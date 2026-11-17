# Changelog

All notable changes to this project are documented in this file.

## 1.0.4 - 2026-11-17

- PHP 8.1 supported again (the previous version required PHP 8.2 by mistake), for Magento 2.4.4 – 2.4.6.

## 1.0.3 - 2026-11-17
- LICENSE file in the package root.
- `module.xml` declares the load order after `Magento_Backend` and `Magento_User` (the extension adds a column to `admin_user` and a field to the user form).
- `composer.json`: explicit version constraints for PHP and the Magento modules it uses.

## 1.0.2
- Fix: an invalid time zone saved on an admin user no longer breaks the admin; the store time zone is used instead.

## 1.0.1 - 2026-06-01
- Bug fixes.

## 1.0.0 - 2026-05-08
- First release: Timezone field on the admin user, applied to the whole backend while that user is logged in.
