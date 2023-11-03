# Welcome to the Craft 4 with Laravel Mix Project.

# Table of Contents

---

1. [Requirements](#installation-requirements)
2. [Build Tools & Assets](#build-tools-&-assets)
3. [Getting Started](#getting-started)
4. [Build Commands](#build-commands)

# Installation requirements

---

* Node.js (at least version 10)
* NPM
* Composer
* Gulp.js version 4

# Tools & Frontend Assets

---

## What's included:
* Craft CMS v4 - Craft is a flexible, user-friendly CMS for creating custom digital experiences on the web and beyond. [Documentation](https://craftcms.com/docs/4.x/)
* Gulp 4 - [Documentation](https://gulpjs.com/docs/en/getting-started/quick-start)
* Laravel Mix - [Documentation](https://laravel-mix.com/)

## Frontend assets:
* Alpine.js v3 - [Documentation](https://alpinejs.dev)
* Tailwind CSS v3 - [Documentation](https://tailwindcss.com/docs)
* Vanilla Lazyload - [Documentation](https://github.com/verlok/vanilla-lazyload/tree/17.1.3)


# Getting Started

---

## Configuring enviroment
Make sure .env variables are updated with the appropriate values. They are used for all frontend build commands. Below are the values used by the frontend build commands.

### `ENVIRONMENT`
Is used to set whether development or production version of files are generated. Expected values are `development`, `dev`, `staging`, or `production`.

### `PRIMARY_SITE_URL`
This is used for browsersync for setting the proxy hostname.

## Configuring paths
### WARNING: Whatever is inside the folder `./web/assets` will be deleted whenever mix commands are ran. This is to prevent caching of old build files. Be careful not to put anything else inside this folder.


## Setting up purging of TailwindCSS 
Make sure in your `package.json` that `"purgeFiles": []` contains an array to any files that contain tailwindcss classes. To learn more go to tailwindcss documentation about (optimizing for production)[https://tailwindcss.com/docs/optimizing-for-production].
 

## Customizing Webpack
Set any custom configuration (e.g. new entry points or other settings) in `webpack.config.js`.

## Favicons
Favicon generation uses Real Favicon Generator. Edit `./faviconConfig.json` to be valid Real [Favicon Generator configuration](https://realfavicongenerator.net/api/non_interactive_api). 

# Build Commands

---

## `npm run build`

## `npm run hot`

## `npm run watch`

## `npm run development`

## `npm run production`

## `npm run critical-css`

## `npm run favicon`
