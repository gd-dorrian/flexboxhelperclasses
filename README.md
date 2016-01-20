## What it is

A CSS (and Sass file) that makes every css flexbox attribute available at every media size - for you to use in HTML. The idea is you can flex display a series of divs, and change the CSS at different media sizes as you see fit without access the CSS. 

## Code Example

<div class="fx-sm-flex-display fx-md-align-content-center fx-sm-align-content-flex-start">
	<div class="inner-div-1"></div>
	<div class="inner-div-2"></div>
	<div class="inner-div-2"></div>
</div>

The above example will add flex-display: flex (with all necessary browser specific prefixes) to the top div element to all screen sizes ABOVE 544px (defined by "-sm" in the Sass file) meaning when you get to mobile size, the div will return to its default CSS. The div will use the flexbox attribute align-content: center (plus all prefixes) to anything above 768px (defined by "fx-md-align-content-center")  once under 768px it will resume the align-content: flex-start  (defined by "fx-sm-align-content-flex-start")  until 544px, then return to default CSS. As you can see it can save you lots of time in writing specific lines in CSS over and over to achieve the same result.

## Extras

If you open the Sass file, you will see we have made the file so you can edit / add / remove media queries as well as setting a custom prefix to all CSS classes if you run into conflicts.
Hope you enjoy!

## Installation

Download > Unzip > Add CSS class to project, OR edit Sass file to suit your project.

## License

GNU General Public License - See license.txt 
