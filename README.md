Grider
======

Grider is an easy to use grid system consisting of settings, mixins and optional classes to provide you a fully functional and responsive layout. With current settings based on the <a href="http://getbootstrap.com/">Bootstrap</a> grid you can now have a quick and full control over your grid system.

## Usage

```
$ git clone git@github.com:jzavrl/grider.git
```

You can either download or clone the repository. After that take out the _grider.scss file and include it into your own Sass structure. Preferable somewhere on the beginning.

## Settings

Grid is fully configurable and very easy to use. You can either use it as mixins inside your Sass code or you can generate classes to use in your markup. Heck, you can use both at the same time if you wish.

```
$grid-unit: px;
$grid-width: 1200px;
$grid-columns: 12;
$grid-gutter: 30px;
```

These are the basics. Unit for the media queries, width for the max width of the grid, number of columns and the size of the gutter. Pretty self explanatory.

```
$grid-generate: true;
```

Wether to generate classes for the grid or not.

```
$grid-container-name: 'container';
$grid-row-name: 'row';
$grid-column-name: 'col-';
$grid-pull-prefix: 'pull-';
$grid-push-prefix: 'push-';
$grid-offset-prefix: 'offset-';
```

Names of the classes. Some will be standalone some will be combined to generate a class such as col-xs-1 or col-xs-push-1.

```
$grid-breakpoints: (
	xs: 0,
	sm: 768,
	md: 992,
	lg: 1200,
);
```

Breakpoint map with key as the part of the class and value for the media queries.
