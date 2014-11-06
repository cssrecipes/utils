# utils

> Some generic, semantic, responsives CSS utilities

## Install

```console
$ npm install cssrecipes-utils
```

```css
@import "./node_modules/cssrecipes-custom-media-queries/index.css";
@import "./node_modules/cssrecipes-utils/index.css"; /* all, max (desktop first) & min (mobile first) versions */
```

## Usage

These utils work well with [cssrecipes-grid](https://github.com/cssrecipes/grid) :

### Mobile-first

```css
@import "./node_modules/cssrecipes-custom-media-queries/index.css";
@import "./node_modules/cssrecipes-utils/all.css";
@import "./node_modules/cssrecipes-utils/min.css";
```

```html
<div class="cssr-Grid">
  <div class="cssr-Grid-cell cssr-all--1of2 cssr-minM--1of3 cssr-minL--1of4">
    <!-- your content-->
  </div>
  <div class="cssr-Grid-cell cssr-all--1of2 cssr-minM--2of3 cssr-minL--3of4">
    <!-- your content-->
  </div>
</div>
```

### Desktop-first

```css
@import "./node_modules/cssrecipes-custom-media-queries/index.css";
@import "./node_modules/cssrecipes-utils/all.css";
@import "./node_modules/cssrecipes-utils/max.css";
```

```html
<div class="cssr-Grid">
  <div class="cssr-Grid-cell cssr-all--1of4 cssr-maxL--1of3 cssr-maxM--1of2">
    <!-- your content-->
  </div>
  <div class="cssr-Grid-cell cssr-all--3of4 cssr-maxL--2of3 cssr-maxM--1of2">
    <!-- your content-->
  </div>
</div>
```

### Without responsive

```css
@import "./node_modules/cssrecipes-utils/all.css";
```

```html
<div class="cssr-Grid">
  <div class="cssr-Grid-cell cssr-all--1of4">
    <!-- your content-->
  </div>
  <div class="cssr-Grid-cell cssr-all--3of4">
    <!-- your content-->
  </div>
</div>
```

## Sizing prefixes

### Default size

- `.cssr-all--XofY`

### Mobile-first

- `.cssr-minS--XofY`
- `.cssr-minM--XofY`
- `.cssr-minL--XofY`
- `.cssr-minXL--XofY`

### Desktop-first

- `.cssr-maxS--XofY`
- `.cssr-maxM--XofY`
- `.cssr-maxL--XofY`
- `.cssr-maxXL--XofY`

## Available sizing

### 2-columns grid

- `*--1of2`
- `*--2of2`

### 3-columns grid

- `*--1of3`
- `*--2of3`
- `*--3of3`

### 4-columns grid

- `*--1of4`
- `*--2of4`
- `*--3of4`
- `*--4of4`

### 5-columns grid

- `*--1of5`
- `*--2of5`
- `*--3of5`
- `*--4of5`
- `*--5of5`

### 6-columns grid

- `*--1of6`
- `*--2of6`
- `*--3of6`
- `*--4of6`
- `*--5of6`
- `*--6of6`

### 8-columns grid

- `*--1of8`
- `*--2of8`
- `*--3of8`
- `*--4of8`
- `*--5of8`
- `*--6of8`
- `*--7of8`
- `*--8of8`

### 10-columns grid

- `*--1of10`
- `*--2of10`
- `*--3of10`
- `*--4of10`
- `*--5of10`
- `*--6of10`
- `*--7of10`
- `*--8of10`
- `*--9of10`
- `*--10of10`

### 12-columns grid

- `*--1of12`
- `*--2of12`
- `*--3of12`
- `*--4of12`
- `*--5of12`
- `*--6of12`
- `*--7of12`
- `*--8of12`
- `*--9of12`
- `*--10of12`
- `*--11of12`
- `*--12of12`

---

## Testing

To generate a build:

```console
$ npm run build
```

To generate the testing build.

```console
$ npm run build-test
```

Basic visual tests are in `test/index.html`.

## Contributing

Work on a branch, install dev-dependencies, respect coding style & run tests before submitting a bug fix or a feature.

```console
$ git clone https://github.com/cssrecipes/utils.git
$ git checkout -b patch-1
$ npm install
$ npm test
```

## [Changelog](CHANGELOG.md)

## [License](LICENSE)
