---
date_modified: 2023-01-27 13:17
date_published: 2015-09-01 19:02
description: Use setup.php in Sage to enable/disable theme features and set configuration values. Register navigation menus, sidebars, define theme support and more.
title: Configuration
authors:
  - alwaysblank
  - ben
  - Log1x
---

# Configuration

## Introduction

All of the configuration for Sage lives inside of `app/setup.php`. Each option is documented allowing for you to easily familiarize yourself with the options configured out of the box.

## Theme Configuration

Configuration specific to WordPress resides in the `app/setup.php` file. In this file, you will find the default enqueued stylesheets and scripts, the supported theme features added with `add_theme_support`, and the registration hooks for navigation menus and sidebars.

By default, Sage is configured to:

- Enqueue `app.css` and `app.js` on the frontend.
- Enqueue `editor.css` and `editor.js` in the Gutenberg editor.
- Add theme support for common functionality.
- Register a default navigation menu called `primary_navigation`.
- Register a primary and footer Sidebar widget area.

### Soil

Also seen in `setup.php` is out of the box theme support for [Soil](https://roots.io/products/soil/) _(recently updated!)_, a WordPress plugin containing a collection of modules applying theme-agnostic front-end modifications including:

- Cleaner WordPress markup
- Disable REST API
- Disable asset versioning
- Disable trackbacks
- Move all Javascript to the footer
- Cleaner NavWalker for navigation menus
- Prettier search URLs converting from `/?s=query` to `/search/query/`
- Root relative URLs

### `theme.json`

Sage ships with a starter `theme.json` that is generated from the build based on your Tailwind config. See the [Gutenberg docs](/sage/docs/gutenberg/) for further information.
