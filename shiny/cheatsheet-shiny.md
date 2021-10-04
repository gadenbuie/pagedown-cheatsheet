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
    number_sections: false
    mathjax: ~
    template: "../template/paged.html"
    css: ["../template/cheatsheet-variables.css", "../template/cheatsheet.css"]
    self_contained: true
    section_div: true
knit: pagedown::chrome_print
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

Amet enim nisi ligula ornare placerat tempor nec est nec nam leo aenean quam! Etiam congue tempus fermentum hendrerit semper urna molestie potenti aenean facilisis. Nascetur sed proin cras netus ullamcorper condimentum. Mattis cum consequat mollis nunc conubia nisl aliquam ante class rutrum. Na rutrum.

Lorem tellus _tellus tortor praesent_ aliquet in `document.getElementById()` neque dictumst. 
Turpis **ullamcorper proin vivamus** suscipit `obj.map(o => o[1])` quisque ante aliquet. 
Fermentum `thoughts.reduce()` libero eleifend molestie!

:::

::: {.box .grid--row-span-2 .box--shaded}
# Heading 1

## Item 1

Adipiscing scelerisque tempus habitant neque neque diam bibendum. Nullam dictumst tellus imperdiet bibendum diam feugiat augue pretium malesuada consequat aenean? Scelerisque egestas sem sociosqu enim sagittis morbi at nulla habitasse dapibus. Eleifend curae tristique mauris volutpat scelerisque arcu urna fusce magna cum sodales varius praesent. Sociis eros et inceptos facilisi elementum laoreet blandit dictumst. Himenaeos curae ridiculus suscipit gravida volutpat per proin tristique ultrices nullam natoque justo. Duis turpis etiam risus tempus libero netus elementum sapien.

## Item 2

Consectetur consequat odio magnis viverra cum curabitur montes porta fringilla feugiat velit.

### Sub Item 1

Lorem sed netus nisl ligula ultrices suspendisse porta euismod? Placerat hendrerit varius iaculis neque tellus proin erat augue tristique class nascetur auctor!

### Sub Item 2

Consectetur curae dis torquent sodales ut orci suscipit! Per torquent odio sodales gravida nibh pharetra sodales vivamus tincidunt sodales id varius condimentum cubilia.
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

Consectetur et sagittis praesent nec cursus odio arcu feugiat penatibus. Neque fringilla eu pretium magna sodales tellus condimentum primis dapibus? Sed primis neque massa conubia nulla varius senectus. Turpis sociosqu rhoncus interdum taciti fringilla ut at hendrerit dictumst? Mus posuere sagittis conubia eget suspendisse dictumst fermentum habitasse. Hac eget faucibus ante aenean tempor erat. Euismod mi commodo arcu interdum scelerisque fermentum natoque malesuada ultricies massa ante integer vivamus faucibus vulputate primis id netus taciti malesuada nibh.

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
