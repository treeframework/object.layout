# Layout

The `layout` system is a powerful, flexible, highly advanced evolution of the
traditional grid system. It is based on
[csswizardry-grids](http://csswizardry.com/csswizardry-grids/).

## Dependencies

The `layout` object depends on two other modules:

* [settings.defaults](https://github.com/treeframework/settings.defaults)
* [tools.functions](https://github.com/treeframework/tools.functions)


If you install the `layout` object using Bower, you will get these dependencies 
at the same time. If not using Bower, please be sure to install and `@import` 
these dependencies in the relevant way.

## Installation

You can install `layout` module via Bower,  npm, or copy and paste.

### Install using Bower:

```sh
$ bower install tree-layout --save
```

Once installed, `@import` into your project in its Object layer:

```scss
@import "bower_components/tree-layout/object.layout";
```

### Install using npm

```sh
$ npm install tree-layout --save
```
### Install via file download

The least recommended option for installation is to simply download
`_object.layout.scss` into your project and `@import` it into your project in 
its Objects layer.

## Usage

Basic usage of the `layout` object uses the required classes:

```html
<div class="o-layout">
    <div class="o-layout__item  u-1/2">...</div><!--
 --><div class="o-layout__item  u-1/2">...</div>
</div>
```

**Note the empty HTML comments.** These are to remove whitespace caused by using
`inline-block`.

## Options

Other, optional classes can supplement the required base classes:

* `.o-layout--[tiny|small|large|huge]`: alter the gutter between layout items.
* `.o-layout--flush`: layouts with no gutters.
* `.o-layout--rev`: reverse rendered order of layout items.
* `.o-layout--[middle|bottom]`: align layout items to the middles or bottoms of each other.
* `.o-layout--right`: make the layout items fill up from the right hand side.
* `.o-layout--center`: make the layout item fill up from the center outward.
* `.o-layout--auto`: cause layout items to take up a non-explicit amount of width.

For example:

```html
<div class="o-layout  o-layout--middle">
    <div class="o-layout__item  u-1/2">I’m in the middle!</div><!--
 --><div class="o-layout__item  u-1/2">I’m in the middle!</div>
</div>
```

## Credits

* **[inuitcss](https://github.com/inuitcss)** Powerful, Sass-based, OOCSS
framework designed with scalability and performance in mind.
