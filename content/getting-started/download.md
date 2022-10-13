---
title: "Download"
date: 2022-10-13T12:06:23+02:00
group: "getting-started"
draft: false
toc: true
---

## Compiled CSS and JS

Download ready-to-use compiled code for **Bootstrap v** to easily drop into your project, which includes:

This doesn't include documentation, source files, or any optional JavaScript dependencies like Popper.

<a  class="btn btn-bd-primary" onclick="ga('send', 'event', 'Getting started', 'Download', 'Download Bootstrap');">Download</a>

## Source files

Compile Bootstrap with your own asset pipeline by downloading our source Sass, JavaScript, and documentation files. This option requires some additional tooling:

- [Sass compiler] for compiling Sass source files into CSS files
- [Autoprefixer](https://github.com/postcss/autoprefixer) for CSS vendor prefixing

Should you require our full set of [build tools], they are included for developing Bootstrap and its docs, but they're likely unsuitable for your own purposes.

<a class="btn btn-bd-primary" onclick="ga('send', 'event', 'Getting started', 'Download', 'Download source');">Download source</a>

## Examples

If you want to download and examine our [examples], you can grab the already built examples:

<a  class="btn btn-bd-primary" onclick="ga('send', 'event', 'Getting started', 'Download', 'Download Examples');">Download Examples</a>

## CDN via jsDelivr

Skip the download with [jsDelivr](https://www.jsdelivr.com/) to deliver cached version of Bootstrap's compiled CSS and JS to your project.

```html
<link rel="stylesheet" crossorigin="anonymous" />
<script crossorigin="anonymous"></script>
```

If you're using our compiled JavaScript and prefer to include Popper separately, add Popper before our JS, via a CDN preferably.

## Package managers

Pull in Bootstrap's **source files** into nearly any project with some of the most popular package managers. No matter the package manager, Bootstrap will **require a [Sass compiler] and [Autoprefixer](https://github.com/postcss/autoprefixer)** for a setup that matches our official compiled versions.

### npm

Install Bootstrap in your Node.js powered apps with [the npm package](https://www.npmjs.com/package/bootstrap):

`const bootstrap = require('bootstrap')` or `import bootstrap from 'bootstrap'` will load all of Bootstrap's plugins onto a `bootstrap` object.
The `bootstrap` module itself exports all of our plugins. You can manually load Bootstrap's plugins individually by loading the `/js/dist/*.js` files under the package's top-level directory.

Bootstrap's `package.json` contains some additional metadata under the following keys:

- `sass` - path to Bootstrap's main [Sass](https://sass-lang.com/) source file
- `style` - path to Bootstrap's non-minified CSS that's been compiled using the default settings (no customization)

### yarn

Install Bootstrap in your Node.js powered apps with [the yarn package](https://yarnpkg.com/en/package/bootstrap):

```sh
yarn add bootstrap@{{}}
```

### RubyGems

Install Bootstrap in your Ruby apps using [Bundler](https://bundler.io/) (**recommended**) and [RubyGems](https://rubygems.org/) by adding the following line to your [`Gemfile`](https://bundler.io/gemfile.html):

Alternatively, if you're not using Bundler, you can install the gem by running this command:

[See the gem's README](https://github.com/twbs/bootstrap-rubygem/blob/master/README.md) for further details.

### Composer

You can also install and manage Bootstrap's Sass and JavaScript using [Composer](https://getcomposer.org/):

### NuGet

If you develop in .NET Framework, you can also install and manage Bootstrap's [CSS](https://www.nuget.org/packages/bootstrap/) or [Sass](https://www.nuget.org/packages/bootstrap.sass/) and JavaScript using [NuGet](https://www.nuget.org/). Newer projects should use [libman](https://docs.microsoft.com/en-us/aspnet/core/client-side/libman/) or another method as NuGet is designed for compiled code, not frontend assets.

```powershell
Install-Package bootstrap
```

```powershell
Install-Package bootstrap.sass
```
