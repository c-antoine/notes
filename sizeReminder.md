# Android java size unit reminder 
## px
 > Pixels - corresponds to actual pixels on the screen.

## in
> Inches - based on the physical size of the screen.
> 1 Inch = 2.54 centimeters

## mm
> Millimeters - based on the physical size of the screen.

## pt
> Points - 1/72 of an inch based on the physical size of the screen.

## dp or dip
> Density-independent Pixels - an abstract unit that is based on the physical density of the screen. These units are relative to a 160 dpi screen, so one dp is one pixel on a 160 dpi screen. The ratio of dp-to-pixel will change with the screen density, but not necessarily in direct proportion. Note: The compiler accepts both "dip" and "dp", though "dp" is more consistent with "sp".

## sp
> Scaleable Pixels OR scale-independent pixels - this is like the dp unit, but it is also scaled by the user's font size preference. It is recommended you use this unit when specifying font sizes, so they will be adjusted for both the screen density and user's preference. Note, the Android documentation is inconsistent on what sp actually stands for, one doc says "scale-independent pixels", the other says "scaleable pixels".
