# figma-autolayout-css

Reproduce the Figma autolayout using CSS classes. Built with SASS.

## How to use it

Import the CSS or SASS file in your project and just CSS classes

#### Generated classes

- `_p-{direction}-{xy-alignment}-{spacing}` : define the behaviour of the autolayout component
  - direction: either row or column
  - xy-alignment: tl (top-left), tc, tr, cl, cc, cr, bl, bc, br
  - spacing: m2, m4, m8, m12, m16, m20, m24, m28
- `_ws` : fill width / hug content is default
- `_hs` : fill height / hug content is default
- `_x{padding}` : padding top and bottom, similar to spacing (\_x2, \_x4, ...)
- `_y{padding}` : padding left and right, similar to spacing (\_y2, \_y4, ...)

#### Example

![example in figma](https://i.ibb.co/qmYKDj0/Clean-Shot-2022-01-26-at-23-13-01-2x.png "Figma autolayout")

    <div className="_p-col-tl-m20 _x12 _y8" style={{background: "yellow"}}>
        <div className="_ws" style={{background: "green"}}>first item</div>
        <div className="_ws" style={{background: "red"}}>second item</div>
    </div>

![example result](https://i.ibb.co/MZrDJfC/Clean-Shot-2022-01-26-at-23-09-01-2x.png "Result in browser")

## Customize

Checkout the instructions in the SASS file to customize the generated classes.
