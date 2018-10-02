# fa5-power-transforms-css
Font Awesome 5 "Power Transform" like functionality using straight CSS


## What is this?

Font Awesome 5 provides some really neat functionality they call Power Transforms.
Power Transforms allow you to shrink icons, rotate icons, and layer icons in endless ways.

The problem is, Power Transforms are only available to users of the SVG + JS version of Font Awesome.
At this time, I prefer the web fonts version for performance reasons.

This project attempts to recreate some of the key Power Transform features in straight CSS.


## Which `data-fa-transform` options are recreated?

`rotate-n`
- Supports whole numbers only, -359 to 359.

`flip-h`, `flip-h`

### `.fa-layers`

The Web Fonts version does offer [stacking](https://fontawesome.com/how-to-use/on-the-web/styling/stacking-icons) using the `.fa-stack` class, but the `.fa-layers` class is far more powerful.

`shrink-n`, `grow-n`
- Supports whole numbers from 1 to 16.

`up-n`, `down-n`, `left-n`, `right-n`
- Supports whole numbers from 1 to 8.

`glow`
- Adds an outline to the icon for some really fancy layering.
- Defaults to white, with some Bootstrap 3 background color options.
- *If you choose to use `glow`, you may need to add your own background color support.*

`data-fa-mask=""`
- Slightly different than the Font Awesome 5 specification.
- The existence of this attribute will **attempt** to set the icon's color to that of the background.
- *If you choose to use `data-fa-mask`, you may need to add your own background color support.*


## I want to see it in action!

[See the examples](https://cityssm.github.io/fa5-power-transforms-css/)
