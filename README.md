# Bootstrap5-addon
> Extra css classes and helpers for bootstrap 5 grid system.

### ASSETS LIST
* [Aspect ratio](#aspect-ratio)
* [Extras](#extras)
* [Images](#images)
* [Links](#links)
* [Minimum Heights](#min-heights)
* [Negative Offsets](#negative-offsets)
* [Typography](#typography)
* [Vertical heights](#vertical-heights)

### HOW TO USE IT

cp node_modules/bootstrap5-addon/sass/_variables.scss ./your/local/folder

## Aspect ratio
For each bootstrap breakpoint adds .ar-$breakpoint-$number class.  
Class `.ar-md-20` will add a 20% padding-top css rule to the given element.  
This will effect the height of the element depending the width, so it will maintain its aspect ratio.  
###### USE
`.ar-$breakpoint-$number`
###### DEFAULT VARIABLES
$number: 5-230 with step 5.  

## Extras
Reset focus outline & .overflow-hidden & .h-100 classes.
###### USE
`.overflow-hidden`  
`.h-100` height 100%  

## Images
Adds width to images.  
Usefull for svg images.  
Use it with bootstrap's .img-fluid class and with caution!
###### USE
`.img-$number`
###### DEFAULT VARIABLES
$number: 5-230 with step 5.  

## Links
Set colors for the links that you will need for your project, in a variables file.
###### USE
.link-$color-name
###### DEFAULT VARIABLES
$link-colors: (
    white:   white,
    black:   black,
    gray:    gray,
    red:     red,
    green:   green,
    blue:    blue,
    yellow:  yellow
)

## Typography
###### USE
`.text-wings`  
`.text-underline`  
`.text-underline-simple`  
`.line-height-$number` ($number: 07-20)  
`.font-weight-$weight`  
`.display-4` & `display-5`  
`.xxlarge`, `.xlarge`, `.large`, `.xsmall`, `.xxsmall`, `.xxxsmall`  
###### DEFAULT VARIABLES

## Vertical heights
###### USE
`.vh-$breakpoints-$number`  
`.vh-max-$breakpoints-$number`  
###### DEFAULT VARIABLES
$number: 5-230 with step 5.  

### VARIABLES
Copy paste this vars in a file.  
Change the variables according to your needs.  
Call this file before the scss assets.

``` scss
/////////////////////////////////////////////////////////////////////////// ASPECT-RATIOS 
$aspect-ratios:             100;
 
/////////////////////////////////////////////////////////////////////////// IMAGES 
$image-widths:              110;

/////////////////////////////////////////////////////////////////////////// MIN HEIGHTS 
$min-heights:               800;
 
/////////////////////////////////////////////////////////////////////////// VERTICAL HEIGHTS 
$vertical-heights:          200;

/////////////////////////////////////////////////////////////////////////// FONT SIZES 
$font-sizes:                0.1;


```

## Contribute
npm version [<newversion> | major | minor | patch | premajor | preminor | prepatch | prerelease [--preid=<prerelease-id>] | from-git]  
npm version [major | minor | patch] -m "Upgrade to %s for reasons"  
npm publish  
