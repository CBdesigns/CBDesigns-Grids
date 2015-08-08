# CBDesigns-Grids

**Simple, fluid, Sass-based, BEM, responsive grid system.**

## Setup

Simply fill in/adjust the relevant variables.

* `$gutter` controls how much space there is between columns.
* `$small-width`, `$medium-width` and `$large-width` controls the breakpoints for the grid.

### Patterns

CBDesigns-Grids’ classes are based on a modified BEM
syntax.

* `.grid` is a **B**lock
* `.grid__item` is an **E**lement
* `.grid--middle` is a **M**odifier

Responsive classes are included to create layouts which work on a range devices. For example:

    <!-- Sets an element to be one half across all breakpoints. -->
    <div class="one-half"></div>

Where as:

    <!-- Sets an element to be one half across all the medium breakpoint. -->
    <div class="one-half@md"></div>

    <!-- Sets an element to be one half across all the small breakpoint. -->
    <div class="one-half@sm"></div>

### Classes in markup

If you are using traditional classes then an example, basic usage might look
like this:

    <div class="grid">
    
        <div class="grid__item  one-half  two-thirds@md">
            ...
        </div>
        <div class="grid__item  one-half  one-thirds@md">
            ...
        </div>
    
    </div>

It’s as simple as that!

---

### Centred grids (`.grid--center{}`)

You can centrally align your grids by simply using the `.grid--center` modifier:

    <div class="grid  grid--center">

        <div class="grid__item  one-half">
            I’m in the middle!
        </div>

    </div>

### Vertically aligned grids (`.grid--[middle|bottom]{}`)

You can vertically align your grids to each other by simply using the
`.grid--[middle|bottom]` modifiers:

    <div class="grid  grid--middle">

        <div class="grid__item  one-half">
            I’m in the middle!
        </div>

        <div class="grid__item  one-half">
            I’m in the middle!
        </div>

    </div>

## Help and questions

If you have any trouble setting CBDesigns-Grids up, or would like some help
using and implementing it (or any questions about how it works) please feel free to [open an issue](https://github.com/CBdesigns/CBDesigns-Grids/issues/new).