## Useful CSS properties that can be used when working with text.

### The system font stack
If you use the `font-family` property to change font and those fonts you are looking for do not happen to be installed on your user’s computer, then a **fallback font** will be displayed. If you have not defined a fallback, then the default HTML font will be used, which is often somewhat ugly. For this reason, it’s common to see somewhat long stacks of fonts listed on projects.

One popular stack is this ‘system font’ stack.

    body {
        font-family: system-ui, "Segoe UI", Roboto, Helvetica, Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
    }

The point of this somewhat ridiculous string of font-families is to try using the default font of the system’s user interface. It will go through each of those fonts until it finds one that is installed on the system, and then use that. Using **a stack like this** often produces *pleasing results*, especially if you’re going for a somewhat *‘neutral’* font style.

### Online font libraries
One popular and easy method to get fonts that are not installed on a user’s computer is to use the online **Font Library**, or the premium, but non-free, **Adobe Fonts**.

>### A warning about Google fonts
>As you look into online font libraries to use you may come across Google Fonts. We strongly advise against using them, as websites that use Google Fonts violate the GDPR.

**To use a font from one of these libraries**, go to the website, select a font and then copy a snippet from the website to import that font from their server into your website. You’ll be given either a `<link>` tag to put in your HTML like so

    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Roboto&display=swap" rel="stylesheet">


or an `@import` tag that can be dropped at the top of a CSS file.

    @import url('https://fonts.googleapis.com/css2?family=Roboto&display=swap');


Keep in mind that it’s **important to add a fallback font**. If you’re linking to an external API, you have no guarantee that the URL won’t change, or that the external API won’t go down at some point. Having a reasonable fallback means that if something goes wrong, at least your site won’t look completely broken.

### Downloaded fonts
It is also possible to use a font that you have **downloaded** from the web. In your CSS file, you import and define a custom font using the `@font-face` rule, and then use it as you would any other font-family.<br>
There are multiple types of font file formats. Please take care when choosing a font file format however, because some *are not universally supported* by browsers. 

    @font-face {
        font-family: my-cool-font;
        src: url(../fonts/the-font-file.woff);
    }

    h1 {
        font-family: my-cool-font, sans-serif;
    }

This method may be more reliable than relying on a third-party font API, but it is always wise to include a fallback.

>Imported font performance considerations.<br>
Like any resource imported fonts must be downloaded by the browser before being used.

## Text styles
There is quite a lot that you can do with **CSS** when it comes to *manipulating text styles*. These rules are all relatively simple and self-explanatory.

### Font-style
Typically used to make a font italic. You learned about the HTML `<em>` tag, which uses an italic font, but `<em>` also signifies that the text it wraps is significant or should be emphasized in some way. A good rule of thumb to follow is that if you just want text to be italic (or bold, underlined, highlighted, etc.), use a CSS property. Otherwise, if text should have some sort of semantic emphasis, use the correct HTML element.

### Letter-spacing
It changes the space between letters in a word. This can be useful for adjusting custom fonts that you feel have too much or too little space. It can also be aesthetically pleasing in some cases, like headers. Obviously, use this sparingly and with care. Do not make your site hard to read!

### Line-height
Adjusts the space between lines in wrapped text. Adding a little line-height can increase readability.

### Text-transform
It changes the case of the given text. You can use this, for example, to force your heading tags to be all uppercase, or to capitalize every word.

### text-shadow
Adds a shadow around the text in the selected element. This one is best used sparingly, but can be used to great effect in headings or other presentational text.

### Ellipsis
This one isn’t a single property, but it’s a **useful trick** to keep in your toolbox. With the text-overflow property, you can truncate overflowing text with an ellipsis. Making an overflow happen, however, requires the use of a couple other properties because the default behavior of text printing outside its container isn’t technically considered an overflow.

    .overflowing {
        white-space: nowrap;
        overflow: hidden;
        text-overflow: ellipsis;
    }





