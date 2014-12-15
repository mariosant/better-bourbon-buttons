Better Bourbon Buttons
======================

Better button mixins for [Bourbon scss framework].

Demo
----

For a look at how everything looks, [check out this page] with code samples and rendered buttons.

[check out this page]: http://mariosant.github.io/bbb-website/

Usage
-----

Include the mixins into your SCSS declarations.

    button.purple {
        // This will create a purple button
        @include bbb_flat_style(#e310eb, white); // Ooooh flat style OTB!
        @include bbb_size(2); // I would like it bigger than usual please
    }

### Available styles

This is a list with the available mixin styles and their usage.

* 3D Style: `@include bbb_3D_style($background-color, $color, $shadow-size);`
* Bordered Style: `@include bbb_bordered_style($border-color, $color);`
* Flat Style: `@include bbb_flat_style($background-color, $color);`
* Simple Style: `@include bbb_simple_style($background-color, $color);`

You can also change the size of the button with the size mixin. It is not obligatory, but it is a very easy way to set button size.

    @include bbb_size(1);  # you can use multipliers to define size
    @include bbb_size(10px);  # or pass the size you want with units

### Expandability / Alternative styles

As Bourbon framework is itself designed to be expanded, the same logic applies to to these mixins. You will find it rather easy to create your own stylings and modify the already defined styles.

Lets create a pill button.

    button.pill {
      @include bbb_simple_style();
      @include bbb_size();
      border-radius: 100px;
    }

Installation
------------

For now, just copy/paste the files into a directory and `@import("better-bourbon-buttons/bbb");`. There will be a better way in the near future.

Contributions
-------------

Contributions are welcome! Please create a pull request.
