## SVG - Scalable Vector Graphics

A very common **image format** on the web, an *incredibly powerful tool* for creating **high-quality, dynamic images** for your website.


### What are SVGs?

A ***scalable*** **image format**, which means they will: 

- **easily scale to any size**
- **retain their quality without increasing their filesize**

and are also very useful if you need to:

- **create or modify your images programmatically** - as you can change their properties through CSS and JavaScript.

**SVGs** are often used for:

1. Icons
2. Graphs/Charts
3. Large, simple images
4. Patterned backgrounds
5. Applying effects to other elements via SVG filters

“**SVG**” stands for “**Scalable Vector Graphics**”.
 
° **Vector graphics** are images defined by *math*<br>
as opposed to traditional<br> 
° “raster graphics” where your image is defined by a *grid of pixels*.

With raster graphics, the detail is *limited to the size of that pixel grid*.<br>
If you want to increase the size of the image (scale it), you have to increase the size of that grid.<br>

*How do you decide what all those new pixels should look like?* There’s no simple solution. Additionally, the larger the grid, the bigger your filesize grows.

With **vector graphics** there’s no grid. Instead, you have **formulas for different shapes and lines**. Since these are just formulas, it doesn’t matter how large or small you want them to appear: **they can scale to any size you want**, and it will have *no effect on the quality or the size of the file*.

**SVGs** have another interesting aspect to them: they’re defined using **XML**.<br>
**XML** (Extensible Markup Language) is an **HTML-like syntax** which is used for lots of things, from APIs, to RSS, to spreadsheet and word editor software.

The fact that **SVG source-code is XML** has a few key `benefits`.

First, it means that it is human-readable. If you were to open up a JPEG in a text editor, it would just look like gobbledygook. If you were to open up an **SVG** it would be with words, tags, attributes. Compared to binary file formats like JPEG, we’re definitely in familiar territory.

The second benefit of XML is that it’s designed to be **interoperable with HTML**, which means you can put the above code directly in an HTML file, without any changes, and it should display the image. And because these can become elements in the DOM just like HTML elements, you can target them with CSS and create them using the Element WebAPI you’ve already been using!

