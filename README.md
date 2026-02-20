# Theme Support Plugin

Customize theme and admin CSS and JS, and load custom Twig templates, blueprints, and Shortcodes.

## Requirements

- Grav CMS >= 1.7.0
- Shortcode Core plugin >= 5.0.0

## Installation

1. Copy the `theme-support` folder into `user/plugins/`
2. The plugin is enabled by default via `theme-support.yaml`

## File Structure

```
theme-support/
├── assets/
│   ├── admin.css       # Admin panel CSS customizations
│   ├── admin.js        # Admin panel JS customizations
│   ├── theme.css       # Frontend theme CSS customizations
│   └── theme.js        # Frontend theme JS customizations
├── blueprints/         # Custom page blueprint (.yaml) files
├── shortcodes/         # Custom shortcode (.php) files
└── templates/          # Custom Twig template (.html.twig) files
```

## Customization

### CSS & JS

Edit the files in `assets/` directly:

- **`admin.css`** — styles applied to the Grav Admin panel
- **`admin.js`** — scripts applied to the Grav Admin panel
- **`theme.css`** — styles applied to the frontend; the included styles target the Helios theme and should be replaced or cleared for other themes
- **`theme.js`** — scripts applied to the frontend; the included script handles Embedly card theming for Helios and should be replaced or cleared for other themes

### Custom Blueprints

Add `.yaml` blueprint files to the `blueprints/` folder. They will be automatically loaded and made available in the Admin panel.

### Custom Shortcodes

Add `.php` shortcode files to the `shortcodes/` folder. They will be automatically registered with the Shortcode Core plugin.

### Custom Twig Templates

Add `.html.twig` template files to the `templates/` folder. They will be added to Twig's template path and can override or extend theme templates.

## License

MIT — Hibbitts Design
