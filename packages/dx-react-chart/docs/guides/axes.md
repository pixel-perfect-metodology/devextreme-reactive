# React Chart - Axes and Grid

The axes and grid improve the visualized data's readability: axes display series point arguments and values; the grid connects series points and axis values.

## Related Plugins

The following plugins implement the axes and grid:

- [ArgumentAxis](../reference/argument-axis.md) - renders an argument axis with grid lines.
- [ValueAxis](../reference/value-axis.md) - renders a value axis with grid lines.
- [Scale](../reference/scale.md) - processes data.

## Basic Setup

Import the plugins listed above to set up a Chart with two axes and a grid.

## Axis Types

The default axis type is linear. It is sutable for numeric data. The following example shows a linear axis:

.embedded-demo({ "path": "chart-basic/default-axis", "showThemeSelector": true })

The band axis type is used to display string values. Set the axis' `type` property to `"band"` as demonstrated in the following example to use a band axis:

.embedded-demo({ "path": "chart-basic/band-axis", "showThemeSelector": true })

## Custom Axis Types

You can also use custom axis types. For this, assign an array of scale configuration objects to the `Scale` plugin's `extensions` property. The following example demonstrates how to use a logarithmic scale with d3 plugins:

.embedded-demo({ "path": "chart-basic/logarithm", "showThemeSelector": true })
