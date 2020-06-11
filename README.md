# EVE Online Fitting Wheel SVG

The EVE Online Fitting Wheel SVG is a fitting wheel commonly used on Killboard within the Eve Online Third Party Community.

### History
Up until the creation of this repo, the fitting wheel was a series of PNGs stacked on top of each other, using inline CSS to position the images inside of a container. Due to these constraints, the image did not fit into a responsive website very well.

## Features

This new Fitting Wheel is an SVG.
Because of this, you can programmatically include, or exclude, any component of the fitting wheel.
Included in the fitting wheel code, 
* Each module is apart of a rack class (i.e. hiSlotRack, medSlotRack, rigRack, subSystemRack, etc)
* Each module/ammo position is grouped under the class of `flag##` where the `#` is the flag id for that position on the ship
* Each module is grouped with its ammo position
* if a module does not have any ammo, css can be used to hide the ammo position. You can set either set the global CSS style of:
 `.flag## > .ammo { display:none }` or you can just programmatically not include the ammo position
