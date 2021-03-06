Angular Material buttons are native `<button>` or `<a>` elements enhanced with Material Design
styling and ink ripples.

<!-- example(button-overview) -->

Native `<button>` and `<a>` elements are always used in order to provide the most straightforward
and accessible experience for users. A `<button>` element should be used whenever some _action_
is performed. An `<a>` element should be used whenever the user will _navigate_ to another view.


There are five button variants, each applied as an attribute:

| Attribute          | Description                                                                 |
|--------------------|-----------------------------------------------------------------------------|
| `md-button`        | Rectangular button w/ no elevation.                                         |
| `md-raised-button` | Rectangular button w/ elevation                                             |
| `md-icon-button`   | Circular button with a transparent background, meant to contain an icon     |
| `md-fab`           | Circular button w/ elevation, defaults to theme's accent color              |
| `md-mini-fab`      | Same as `md-fab` but smaller                                                |


### Theming
Buttons can be colored in terms of the current theme using the `color` property to set the
background color to `primary`, `accent`, or `warn`. By default, only FABs (Floating Action Button) 
are colored; the default background color for `md-button` and `md-raised-button` matches the theme's 
background color.

### Capitalization
According to the Material design spec button text has to be capitalized, however we have opted not
to capitalize buttons automatically via `text-transform: uppercase`, because it can cause issues in
certain locales. It is also worth noting that using ALL CAPS in the text itself causes issues for
screen-readers, which will read the text character-by-character. We leave the decision of how to
approach this to the consuming app.
