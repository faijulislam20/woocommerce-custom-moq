
# WooCommerce Custom MOQ

**Product & Variation-Level Minimum Order Quantity Management for WooCommerce**

A WordPress plugin project designed to help WooCommerce store owners manage minimum order quantities (MOQ) for individual products and product variations.

**Project Status:** Planning & Development  
**Maintainer:** Md. Faijul Islam  
**Repository:** https://github.com/faijulislam20/woocommerce-custom-moq

> ⚠️ This project is under development. No production-ready plugin is available yet. Do not install or use it on a live store.

---

## Overview

Minimum Order Quantity (MOQ) is the smallest number of units a customer must purchase for a product or variation.

MOQ rules are particularly useful for wholesale suppliers, manufacturers, B2B businesses, and bulk-order eCommerce stores.

This project aims to provide a maintainable WooCommerce solution for configuring and validating product-specific and variation-specific minimum quantities.

## The Problem

WooCommerce stores serving bulk buyers may require different minimum purchase quantities for different products.

For example:

| Product | Example MOQ |
|---|---:|
| Leather Wallet | 30 pieces |
| Backpack | 50 pieces |
| Shopping Bag | 100 pieces |
| Custom T-Shirt | 50 pieces |
| Promotional Cap | 100 pieces |

These are illustrative business rules, not default plugin settings.

Store owners need a way to manage these requirements while preventing orders below the configured minimum.

## Planned Features

The following features are development targets and are not yet implemented.

- Product-level minimum order quantity settings
- Variation-specific MOQ configuration
- Admin-editable MOQ fields
- Quantity input minimum and initial value
- Quantity increment of 1
- Add-to-cart quantity validation
- Cart quantity update validation
- Clear customer-facing error messages
- Compatibility testing with classic WooCommerce flows
- Compatibility testing with WooCommerce Cart and Checkout Blocks

## Example: Variation-Level MOQ

A variable product may have different minimum quantities for each variation.

| Variation | Example Minimum |
|---|---:|
| Black | 30 |
| Brown | 50 |
| Blue | 40 |

If a customer selects the Black variation, the planned behavior is to start the quantity at 30 and reject quantities below 30.

The same validation must be enforced on the server, not only through the browser's quantity input.

## Planned Technical Approach

The project will explore WooCommerce's documented quantity input filters, product and variation metadata, and cart validation mechanisms.

Implementation will consider:

1. WordPress and WooCommerce coding standards
2. Secure admin field handling
3. Input validation and sanitization
4. Proper output escaping
5. Classic cart and Store API differences
6. Product variation behavior
7. Stock and purchasability restrictions
8. Compatibility and regression testing

## Development Roadmap

| Phase | Task | Status |
|---|---|---|
| 1 | Requirements and technical research | In progress |
| 2 | Plugin structure and bootstrap | Planned |
| 3 | Product-level MOQ settings | Planned |
| 4 | Variation-level MOQ settings | Planned |
| 5 | Quantity input integration | Planned |
| 6 | Add-to-cart and cart validation | Planned |
| 7 | Security and compatibility testing | Planned |
| 8 | Documentation and initial release | Planned |

## Installation

**Installation is not available yet.**

This repository currently documents a planned plugin.

Installation instructions will be published only after an installable build has been created and tested.

## Compatibility

WordPress, PHP, and WooCommerce minimum supported versions have not yet been established.

Compatibility claims will be added after testing against specific versions and store configurations.

## Testing Plan

Before the first stable release, the project should test:

- Simple products
- Variable products
- Variation-specific MOQ values
- Quantities below the minimum
- Quantities equal to the minimum
- Quantities above the minimum
- Cart quantity updates
- Classic cart behavior
- Cart and Checkout Blocks
- Invalid or missing MOQ settings
- Stock and backorder interactions
- Guest and logged-in customer flows

Test results and known limitations will be documented.

## Security

The implementation will follow relevant WordPress and WooCommerce security practices.

No API keys, passwords, customer records, or private business information should be committed to this repository.

Security issues should be reported privately to the maintainer rather than disclosed publicly before review.

## Frequently Asked Questions

### What is a Minimum Order Quantity?

MOQ is the minimum number of units a customer must purchase for a product or variation.

### Does WooCommerce Custom MOQ work with variable products?

Variation-level MOQ support is planned but has not yet been implemented or tested.

### Can store owners set different minimum quantities?

Product-specific and variation-specific settings are planned features.

### Is this plugin ready for production?

No. The project is currently in the planning and development stage.

### Will it support WooCommerce Cart and Checkout Blocks?

Compatibility with block-based cart and checkout flows is part of the planned testing scope.

## Official Technical References

- [WooCommerce Developer Documentation](https://developer.woocommerce.com/)
- [WooCommerce Quantity Input Values](https://developer.woocommerce.com/docs/code-snippets/adjust-quantity-input-values/)
- [WooCommerce Store API Cart Documentation](https://developer.woocommerce.com/docs/apis/store-api/resources-endpoints/cart/)
- [WordPress Plugin Handbook](https://developer.wordpress.org/plugins/)
- [GitHub README Documentation](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes)

## Maintainer

**Md. Faijul Islam**

WordPress & WooCommerce Development | Entrepreneurship | Digital Business

GitHub: https://github.com/faijulislam20

Website: https://fsbmanufacturingltd.com

Email: fsbmanufacturingltd@gmail.com

## License

A license has not yet been selected. Until a license is added, no open-source reuse permission is granted by this repository.

---

**Development philosophy:** Research carefully. Build responsibly. Test thoroughly. Document clearly.
