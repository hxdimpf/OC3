# OC3 — OpenCaching Legacy Application

The original PHP application powering opencaching.de. PHP 8.2, 
Smarty templates, MariaDB.

## Quick Start

    git clone git@github.com:hxdimpf/OC3.git
    cd OC3
    ddev start

The app is running at `https://oc3.ddev.site`.

## Structure

- `app/` — Symfony 3.x (legacy) application kernel and config
- `config2/` — OC2 configuration files
- `lib2/` — legacy PHP libraries (common.inc.php, web.inc.php, etc.)
- `templates2/` — Smarty templates (ocstyle)
- `lang/` — translation files
- `api/` — API endpoints
- `util/` — utility scripts (cron jobs, maintenance)
- `bin/` — CLI tools
- `assets/` — static JavaScript/CSS

## Bridge to OC4

The `assets/oc-new-ui-toggle.js` file redirects specific pages
to the [OC4 Symfony frontend](https://github.com/hxdimpf/OC4).
Add routes to the mapping table as OC4 pages come online.

## License

See [LICENSE.md](LICENSE.md).
