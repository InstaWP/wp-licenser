# WP License Activations

🔑 A WP‑CLI utility to activate and manage licenses for popular WordPress plugins and themes. Supports automation, provisioning, and bulk site setup workflows.

> This project will evolve into a full WP‑CLI package to provide a unified interface for license activation across the WordPress ecosystem. As of now, we are collecting various commands or methods already exist to activate pro licenses. 

---

## ✅ Supported via WP-CLI

| Plugin/Theme       | WP-CLI Command Example |
|--------------------|------------------------|
| **Elementor Pro**  | `wp elementor-pro license activate <license-key>` |
| **WP Rocket**      | `wp rocket activate <license-key>` |
| **Gravity Forms**  | `wp gf license <license-key>` *(requires WP-CLI addon)* |
| **WPML**           | `wp wpml register <site-key>` |
| **Polylang Pro**   | `wp pll license activate <license-key>` |
| **SEOPress Pro**   | `wp seopress license activate <license-key>` |
| **MainWP**         | `wp mainwp child connect` *(license handled via parent site)* |

---

## ⚠️ Partial or Indirect Support

| Plugin/Theme             | Notes |
|--------------------------|-------|
| **ACF Pro**              | No official CLI, but `wp option update` or `.env` tricks may work |
| **The Events Calendar**  | No CLI; uses transient auth |
| **Divi (Elegant Themes)**| Manual UI activation; license stored in `et_` options |
| **Envato/ThemeForest**   | No CLI; activation via Envato API or Toolkit plugin |



