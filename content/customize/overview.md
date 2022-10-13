---
title: "Overview"
date: 2022-10-13T12:06:23+02:00
group: "customize"
draft: false
toc: true
---

## Overview

There are multiple ways to customize Bootstrap. Your best path can depend on your project, the complexity of your build tools, the version of Bootstrap you're using, browser support, and more.

Our two preferred methods are:

1. Using Bootstrap [via package manager]({{}}) so you can use and extend our source files.
2. Using Bootstrap's compiled distribution files or [jsDelivr]({{}}) so you can add onto or override Bootstrap's styles.

While we cannot go into details here on how to use every package manager, we can give some guidance on [using Bootstrap with your own Sass compiler]({{}}).

For those who want to use the distribution files, review the [getting started page]({{}}) for how to include those files and an example HTML page. From there, consult the docs for the layout, components, and behaviors you'd like to use.

As you familiarize yourself with Bootstrap, continue exploring this section for more details on how to utilize our global options, making use of and changing our color system, how we build our components, how to use our growing list of CSS custom properties, and how to optimize your code when building with Bootstrap.

## CSPs and embedded SVGs

Several Bootstrap components include embedded SVGs in our CSS to style components consistently and easily across browsers and devices. **For organizations with more strict <abbr title="Content Security Policy">CSP</abbr> configurations**, we've documented all instances of our embedded SVGs (all of which are applied via `background-image`) so you can more thoroughly review your options.

- [Accordion]({{}})
- [Carousel controls]({{}})
- [Close button]({{}}) (used in alerts and modals)
- [Form checkboxes and radio buttons]({{}})
- [Form switches]({{}})
- [Form validation icons]({{}})
- [Navbar toggle buttons]({{}})
- [Select menus]({{}})

Based on [community conversation](https://github.com/twbs/bootstrap/issues/25394), some options for addressing this in your own codebase include [replacing the URLs with locally hosted assets]({{}}), removing the images and using inline images (not possible in all components), and modifying your CSP. Our recommendation is to carefully review your own security policies and decide on the best path forward, if necessary.
