# Sass

Use [scss-lint](https://github.com/brigade/scss-lint) to keep SCSS files clean and readable.    
Include file [.scss-lint.yml](.scss-lint.yml) in the current working directory.     
A git [pre-commit hook](../git/hooks/pre-commit) should be used to run scss-lint before each commit.


## Formatting

* Use the SCSS syntax.
* Use a single space before and no space after the !
* Use hyphens when naming mixins, extends, classes, functions & variables: `span-columns` not `span_columns` or `spanColumns`.
* Use one space between property and value: `width: 20px` not `width:20px`.
* Prefer hex color codes `#fff`.
* Prefer color: #fff instead of color: white
* Use `//` for comment blocks not `/* */`.
* Use one space between selector and `{`.
* Use double quotation marks.
* Use only lowercase, except for hex or string values.
* Don't add a unit specification after `0` values, unless required by a mixin.
* Use a leading zero in decimal numbers: `0.5` not `.5`
* Use space around operands: `$variable * 1.5`, not `$variable*1.5`
* Use a `%` unit for the amount/weight when using Sass's color functions: `darken($color, 20%)`, not `darken($color, 20)`
* Use multi-line CSS
* Use shorthand properties where possible

## Order

* Use alphabetical order for declarations.
* Place `@extends` and `@includes` at the top of your declaration list.
* Place media queries directly after the declaration list.
* Place concatenated selectors second.
* Place pseudo-states and pseudo-elements third.
* Place nested elements fourth.
* Place nested classes fifth.

## Selectors

* Don't use ID's for style.
* Use meaningful names: `$visual-grid-color` not `$color` or `$vslgrd-clr`.
* Avoid nesting more than 4 selectors deep.
* Don't nest more than 6 selectors deep.
* Avoid using HTML tags on classes for generic markup `<div>`, `<span>`: `.widgets` not `div.widgets`.
* Avoid using HTML tags on classes with specific class names like `.featured-articles`.

## Organization

* Avoid having files longer than 100 lines.
