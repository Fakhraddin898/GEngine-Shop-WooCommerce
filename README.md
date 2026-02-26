# G-Engine Woocommerce Plugin

A WordPress + WooCommerce plugin that integrates the **G-Engine API** (`api.g-engine.net/v2.1`) to power a full-featured Azerbaijani game top-up and gift card shop — with AZN pricing, custom shortcodes, product sync, and live order processing.

---

## Features

- **G-Engine API Integration** — Connects to `https://api.g-engine.net/v2.1` for product data and order submission
- **AZN Currency Support** — Built-in AZN rate conversion (default: 1.7)
- **Shortcodes** — Three ready-to-use shortcodes for embedding the shop anywhere on your site
- **Product Sync** — Sync G-Engine products into WordPress as custom post types
- **Add to Cart (AJAX)** — Fast, seamless add-to-cart without page reloads
- **Game Recharge** — Dedicated recharge shortcode for top-up products
- **Gift Cards** — Separate gift card section with its own shortcode
- **Checkout Meta** — Game-specific fields (User ID, Server, etc.) saved per order line item
- **Order Processing** — Automatically submits orders to G-Engine API on `processing` and `completed` status
- **Custom Product Images** — Save and manage product images via admin AJAX
- **Search Support** — G-Engine custom post types appear in WordPress search results
- **New Blue Design** — Modern, clean UI included

---

## Shortcodes

| Shortcode | Description |
|---|---|
| `[gengine_shop]` | Main shop listing with all products |
| `[gengine_recharge]` | Top-up / recharge products |
| `[gengine_gift_cards]` | Gift card products |

---

## Requirements

- WordPress 5.6+
- WooCommerce 5.0+
- PHP 7.4+
- A valid **G-Engine API** account and key

---

## Installation

1. Download the latest release (`gengine-azn-shop-v3_3-FINAL.zip`) from the [Releases](../../releases) page.
2. In your WordPress admin panel, go to **Plugins → Add New → Upload Plugin**.
3. Upload the zip file and click **Install Now**, then **Activate**.
4. Go to **G-Engine Settings** in the admin menu and enter your API key.

---

## Configuration

| Setting | Description |
|---|---|
| API URL | `https://api.g-engine.net/v2.1` |
| API Key | Your G-Engine account API key |
| AZN Rate | Conversion rate (default: `1.7`) |

---

## How It Works

1. **Sync products** from G-Engine API into WordPress custom post type `gengine_product`
2. Customers browse the shop via shortcodes on any page
3. On checkout, game-specific fields (User ID, Zone/Server) are collected and saved to the order
4. When the order reaches **Processing** or **Completed** status, the plugin automatically calls the G-Engine API to fulfill the order

---

## Changelog

### v3.3 FINAL (v3.2-AZ-IMPROVED)
- Full G-Engine API v2.1 integration
- AZN currency with configurable rate
- Three shortcodes: shop, recharge, gift cards
- AJAX add-to-cart and product sync
- Custom post type with search support
- Order auto-fulfillment via G-Engine API
- New modern blue design

---

## Author

**Fakhraddin Ahmadov** (Faxri) — built with assistance from Manus AI.

---

## License

For personal and commercial use. Please review [G-Engine API Terms](https://g-engine.net) before deploying in production.
