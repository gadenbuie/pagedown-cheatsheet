---
title: "Customizing Shiny"
author: "Garrick Aden-Buie"
description: >
  Using custom inputs and interactivity with JavaScript in Shiny apps
logo: shiny-logo.svg
columns: 4
date: "2021-10-04"
output:
  pagedown::html_paged:
    keep_md: true
    mathjax: ~
    template: "../template/paged.html"
    css: ["../template/cheatsheet-variables.css", "../template/cheatsheet.css"]
    self_contained: true
    section_div: true
---



<style type="text/css">
@page {
  @bottom-right {
    content: "test";
  }
}
</style>

::: box

## Adding dependencies

- `htmltools::htmlDependency()`

- `createWebDependency()`

- `addResourcePath()`

- `includeScript()`, `includeCSS()`
:::

::: {.box .grid--col-span-2}
# Heading 1

Ipsum ullamcorper at augue nascetur! Scelerisque platea facilisi sollicitudin feugiat malesuada velit litora proin molestie proin metus! Nibh erat netus sociis mus maecenas fames viverra lacinia semper leo facilisis.

Lorem tellus _tellus tortor praesent_ aliquet in `document.getElementById()` neque dictumst. 
Turpis **ullamcorper proin vivamus** suscipit `obj.map(o => o[1])` quisque ante aliquet. 
Fermentum `thoughts.reduce()` libero eleifend molestie!

:::

::: {.box .grid--row-span-2 .box--shaded}
# Heading 1

## Item 1

Sit est convallis turpis ultrices dis urna quisque. Nulla dui tellus fringilla est torquent fringilla condimentum litora class.

## Item 2

Adipiscing nisl pretium libero lectus in augue?

### Sub Item 1

Amet fringilla morbi fusce volutpat gravida vulputate proin dignissim euismod netus. Fermentum nisi pretium quisque aliquam magna a pretium hac integer volutpat.

### Sub Item 2

Consectetur nibh commodo nec montes nascetur netus justo iaculis venenatis. Facilisis cras scelerisque eros purus condimentum parturient parturient!
:::

::: {.box .box--bordered .box--border-dashed}

# DOM

## Find DOM Elements

```html
<button id="sumbit" class="btn"></button>
```


|<code>document</code>      |Example input |
|:--------------------------|:-------------|
|`.getElementById()`        |`'submit'`    |
|`.getElementByClassName()` |`'btn'`       |
|`.getElementByTagName()`   |`'button'`    |
|`.querySelector()`         |`'.btn'`      |
|`.querySelectorAll()`      |`'button'`    |

:::

::: box

# Box Title 1

## Sub Title 1

Sit nam vestibulum praesent id rutrum pellentesque ante. Quis nulla habitasse senectus potenti at vehicula dui at accumsan felis fames. Fermentum dignissim lacinia nostra cras suspendisse enim sagittis aliquam nisl mauris. Integer volutpat imperdiet sociosqu vestibulum pretium ante! Velit ultrices etiam scelerisque ultricies molestie gravida facilisi ad gravida etiam hac proin molestie.

$$e = mc^2$$

:::

::: {.box .box--inverted}

# Box Title 1

## Sub Title 1

Elit sociosqu laoreet *bibendum inceptos elementum integer* primis nulla curae aenean nulla imperdiet? **Risus primis facilisi** integer magna lobortis nec sagittis accumsan nullam cras fusce dapibus? Eros vestibulum `class libero at mauris potenti a ultrices` curabitur nullam molestie varius molestie! 

:::


::: {.box}

# Box Title 1

## Sub Title 1

```js
Array.prototype.from();
document.getElementById('test');
```

:::
