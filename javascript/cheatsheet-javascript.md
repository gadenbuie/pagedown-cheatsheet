---
title: "JavaScript"
author: "Garrick Aden-Buie"
description: >
  The event-driven, functional, imperative, object-oriented 
  programming language that runs the web
logo: javascript-logo.svg
columns: 4
date: "2021-10-04"
output:
  pagedown::html_paged:
    keep_md: true
    number_sections: false
    mathjax: ~
    template: "paged.html"
    css: ["cheatsheet-variables.css", "cheatsheet.css"]
    # change to true for a self-contained document, but it'll be a litte slower for Pandoc to render
    self_contained: false
    section_div: true
---




::: box

# Functions

## Classic Functions

```js
function inc(x, by = 1) {
  return x + by
}
const inc = function(x, by = 1) {
  return x + by
}
```

## Arrow Functions

```js
const inc = (x, by = 1) => {
  return x + by
}
const inc = (x, by = 1) => x + by
const incOne = x => x + 1
```
:::

::: {.box}

# Object Literals & Constructors

|Literal           |`typeof`     |Constructor  |
|:-----------------|:------------|:------------|
|`1`               |`'number'`   |`Number()`   |
|`3.14`            |`'number'`   |`Number()`   |
|`'some text'`     |`'string'`   |`String()`   |
|`[]`              |`'object'`   |`Array()`    |
|`{}`              |`'object'`   |`Object()`   |
|`true`            |`'boolean'`  |`Boolean()`  |
|`function f() {}` |`'function'` |`Function()` |

:::

::: {.box}

# Array Methods

| Task | Method | Modifies |
|:----|:------|:----------------|
| Add to a stack (LIFO) | <code>push</code> | in-place
| Get from stack (LIFO) | <code>pop</code> | in-place
| Add to queue (FIFO) | <code>unshift</code> | in-place
| Get from queue (FIFO) | <code>shift</code> | in-place
| Add multiple elements at the end | <code>concat</code> | copy
| Get subarray | <code>slice</code> | copy
| Add or remove elements at position | <code>splice</code> | in-place
| Cut and replace within array | <code>copyWithin</code> | in-place
| Fill an array | <code>fill</code> | in-place
| Reverse an arary | <code>reverse</code> | in-place
| Sort an array | <code>sort</code> | in-place

:::

::: {.box .grid--row-span-2}

# Math

A built-in object with properties and methods for math operations.

## Properties

| `Math` | Value |
|:---|:---|
| `.PI` | $\pi$ |
| `.E` | Euler's constant |
| `.LN2` | Natural logarithm of 2 |
| `.LN10` | Natural Logarithm of 10 |
| `.LOG2E` | Base 2 Logarithm of _e_ |

## Methods

| `Math` | Value |
|:--|:--|
| `.abs(x)` | Absolute value |
| `.cbrt(x)` | Cube root |
| `.ceil(x)`, `.floor(x)` | Integer _ceiling_, _floor_ |
| `.exp(x)` | $e^x$ |
| `.log(x)`, `.log1p(x)`, `.log10(x)`, `.log2(x)` | $ln()$, $ln(1 + x)$, <br>$log_{10}(x)$, $log_2(x)$ |
| `.max(...x)`, `.min(...x)` | Max and min value |
| `.pow(x, y)` | $x^y$ |
| `.random()` | Unif. random # in [0, 1] |
| `.round(x)` | Round to nearest integer |
| `.sign(x)` | Sign of x |
| `.trunc(x)` | Integer part of x |
| `.sin(x)`, `.sinh(x)`, `.cos(x)`, `.cosh(x)` `.tan(x)`, `.tanh(x)` | Trigonometric functions |
| `.asin(x)`, `.asinh(x)`, `.acos(x)`, `.acosh(x)` `.atan(x)`, `.atanh(x)` | Inverse trigonometric functions |

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

Adipiscing nascetur quisque at feugiat feugiat eros pharetra pulvinar dictum. Duis dui molestie urna vitae bibendum pharetra iaculis interdum pharetra non et. Vestibulum dapibus ridiculus habitant erat!

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

<style type="text/css">
:root {
  --text-light: #eaecee;
}

/* Table Elements */
table {
  border-collapse: collapse;
  width: 100%;
  max-width: 100%;
}

table tbody tr:nth-child(2n) {
  background-color: var(--text-light);
}

table,
table th,
table td {
  vertical-align: top;
}
</style>
