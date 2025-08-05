# WP License Activations

🔑 A WP‑CLI utility to activate and manage licenses for popular WordPress plugins and themes. Supports automation, provisioning, and bulk site setup workflows.

> This project will evolve into a full WP‑CLI package to provide a unified interface for license activation across the WordPress ecosystem. As of now, we are collecting various commands or methods already exist to activate pro licenses. 

---

## ✅ Supported via WP‑CLI or Constants

| Plugin/Theme         | Method                           | Activation Command or Snippet |
|----------------------|----------------------------------|-------------------------------|
| **Elementor Pro**    | WP-CLI                           | `wp elementor-pro license activate <license-key>` |
| **WP Rocket**        | Constant                         | Define `WP_ROCKET_EMAIL` and `WP_ROCKET_KEY` in `wp-config.php` |
| **Gravity Forms**    | WP-CLI Addon / Constant          | `wp gf license update <license-key>` or define `GF_LICENSE_KEY` |
| **WPML**             | WP-CLI                           | `wp wpml register <site-key>` |
| **Polylang Pro**     | WP-CLI                           | `wp pll license activate <license-key>` |
| **SEOPress Pro**     | WP-CLI                           | `wp seopress license activate <license-key>` |
| **Astra Pro**        | WP-CLI                           | `wp brainstormforce license activate astra-addon <license-key>` |
| **Beaver Builder**   | WP-CLI / Constant                | `wp beaver register --license=<key>` or define `FL_LICENSE_KEY` |
| **ACF Pro**          | Constant / WP-CLI (eval)         | Define `ACF_PRO_LICENSE` or use `wp eval "acf_pro_update_license('<key>')"` |
| **WPForms**          | Constant                         | Define `WPFORMS_LICENSE_KEY` in `wp-config.php` |
| **Toolset**          | Constant                         | Define `OTGS_INSTALLER_SITE_KEY_TOOLSET` in `wp-config.php` |
| **Neve Pro**         | WP-CLI                           | `wp neve activate <license-key>` |
| **Meta Box**         | Constant                         | Define `META_BOX_KEY` in `wp-config.php` |

---

## ⚠️ Partial or Indirect Support

| Plugin/Theme             | Notes |
|--------------------------|-------|
| **Divi (Elegant Themes)**| Supports constants `ET_USERNAME` and `ET_API_KEY` in `wp-config.php`; no CLI |
| **The Events Calendar**  | License stored in transients; no WP-CLI or constants supported |
| **Envato/ThemeForest**   | Requires Envato Market plugin; no WP-CLI, handled via OAuth |
| **OceanWP**              | Manual activation only; no CLI or programmatic method |
| **Kadence Pro**          | Activation via UI only; some constants available but undocumented |
| **Bricks Builder**       | Activation via UI; no official CLI or API method |
| **Breakdance Builder**   | No documented CLI/API methods; UI activation only |
| **Thrive Suite**         | SaaS-locked license; must authenticate via dashboard UI |
