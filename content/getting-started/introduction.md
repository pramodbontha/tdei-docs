---
title: "Introduction"
date: 2022-10-13T12:06:07+02:00
group: "getting-started"
draft: false
toc: true
---

## Quick start

Get started by including Bootstrap's production-ready CSS and JavaScript via CDN without the need for any build steps. See it in practice with this [Bootstrap CodePen demo](https://codepen.io/team/bootstrap/pen/qBamdLj).  
This is Rakesh Testing the online collaboration

<br>

1. **Create a new `index.html` file in your project root.** Include the `<meta name="viewport">` tag as well for [proper responsive behavior](https://developer.mozilla.org/en-US/docs/Web/HTML/Viewport_meta_tag) in mobile devices.

   ```html
   <!DOCTYPE html>
   <html lang="en">
     <head>
       <meta charset="utf-8" />
       <meta name="viewport" content="width=device-width, initial-scale=1" />
       <title>Bootstrap demo</title>
     </head>
     <body>
       <h1>Hello, world!</h1>
     </body>
   </html>
   ```

2. **Include Bootstrap's CSS and JS.** Place the `<link>` tag in the `<head>` for our CSS, and the `<script>` tag for our JavaScript bundle (including Popper for positioning dropdowns, poppers, and tooltips) before the closing `</body>`. Learn more about our [CDN links](#cdn-links).

   ```html
   <!DOCTYPE html>
   <html lang="en">
     <head>
       <meta charset="utf-8" />
       <meta name="viewport" content="width=device-width, initial-scale=1" />
       <title>Bootstrap demo</title>
     </head>
     <body>
       <h1>Hello, world!</h1>
     </body>
   </html>
   ```

   You can also include [Popper](https://popper.js.org/) and our JS separately. If you don't plan to use dropdowns, popovers, or tooltips, save some kilobytes by not including Popper.

3. **Hello, world!** Open the page in your browser of choice to see your Bootstrapped page. Now you can start building with Bootstrap by creating your own [layout], adding dozens of [components]

## CDN links

As reference, here are our primary CDN links.

You can also use the CDN to fetch any of our [additional builds listed in the Contents page].

## Next steps

- Read a bit more about some [important global environment settings](#important-globals) that Bootstrap utilizes.

- Read about what's included in Bootstrap in our [contents section]and the list of [components that require JavaScript](#js-components) below.

- Need a little more power? Consider building with Bootstrap by [including the source files via package manager].

- Looking to use Bootstrap as a module with `<script type="module">`? Please refer to our [using Bootstrap as a module] section.

## JS components

Curious which components explicitly require our JavaScript and Popper? Click the show components link below. If you're at all unsure about the general page structure, keep reading for an example page template.

<details>
<summary class="text-primary mb-3">Show components requiring JavaScript</summary>

</details>

## Important globals

Bootstrap employs a handful of important global styles and settings, all of which are almost exclusively geared towards the _normalization_ of cross browser styles. Let's dive in.

### HTML5 doctype

Bootstrap requires the use of the HTML5 doctype. Without it, you'll see some funky and incomplete styling.

```html
<!DOCTYPE html>
<html lang="en">
  ...
</html>
```

### Responsive meta tag

Bootstrap is developed _mobile first_, a strategy in which we optimize code for mobile devices first and then scale up components as necessary using CSS media queries. To ensure proper rendering and touch zooming for all devices, add the responsive viewport meta tag to your `<head>`.

```html
<meta name="viewport" content="width=device-width, initial-scale=1" />
```

You can see an example of this in action in the [quick start](#quick-start).

### Box-sizing

For more straightforward sizing in CSS, we switch the global `box-sizing` value from `content-box` to `border-box`. This ensures `padding` does not affect the final computed width of an element, but it can cause problems with some third-party software like Google Maps and Google Custom Search Engine.

On the rare occasion you need to override it, use something like the following:

```css
.selector-for-some-widget {
  box-sizing: content-box;
}
```

With the above snippet, nested elements—including generated content via `::before` and `::after`—will all inherit the specified `box-sizing` for that `.selector-for-some-widget`.

Learn more about [box model and sizing at CSS Tricks](https://css-tricks.com/box-sizing/).

### Reboot

For improved cross-browser rendering, we use [Reboot] to correct inconsistencies across browsers and devices while providing slightly more opinionated resets to common HTML elements.

## Community

Stay up-to-date on the development of Bootstrap and reach out to the community with these helpful resources.

- Ask and explore [our GitHub Discussions](https://github.com/twbs/bootstrap/discussions).
- Chat with fellow Bootstrappers in IRC. On the `irc.libera.chat` server, in the `#bootstrap` channel.
- Implementation help may be found at Stack Overflow (tagged [`bootstrap-5`](https://stackoverflow.com/questions/tagged/bootstrap-5)).
- Developers should use the keyword `bootstrap` on packages that modify or add to the functionality of Bootstrap when distributing through [npm](https://www.npmjs.com/search?q=keywords:bootstrap) or similar delivery mechanisms for maximum discoverability.
