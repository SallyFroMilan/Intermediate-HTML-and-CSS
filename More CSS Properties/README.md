## Useful little CSS features you can use to add some shine to your projects.
There are a lot of CSS properties, *hundreds*. Luckily, you don’t have to memorize them all: the amount of properties you’re actually going to use on a daily basis is much smaller.

## Background
The background property not only sets background colors but is actually a shorthand for 8 different background-related properties:
<ul>
<li>specify background images</li>
<li>change the position of background images</li>
<li>change the size of background images</li>
<li>change how background images repeat</li>
<li>or tile if they are too small to fill their container</li>
<li>have multiple background layers</li>
</ul>

One thing to note is that it is possible to use these properties **individually**, and in some cases it might be *easier and more clear* to do that than defaulting to the shorthand. This is in contrast to some other shorthand properties where it is almost always preferable to default to using the shorthand (flex, margin, padding etc.).

## Borders
You’ve already encountered `border` and `border-radius`.<br>
The `border` property is another shorthand, but it is much less complicated than the background shorthand. For borders, basically you just need to define a size, style and color.

`border-radius` is the property that is used to create rounded corners on things. It’s possible to get fancy and define different radii for each corner of an element, but this is rarely useful.

## Box-shadow
It adds a shadow effect around an element. This is useful to create a sense of depth on your page and to add subtle separation between elements.

In usage it’s straightforward, but keep in mind that it’s best used sparingly, and subtly. Prefer lighter, barely visible shadows to darker or brighter colors.

## Overflow
It is possible, using overflow, to define what happens to an element when its content is too big to fit. The most common usage is likely to add scrollbars to an element inside a webpage, for example a card style element with scrollable content.

## Opacity
Opacity is another easy one that can be very useful in some circumstances.