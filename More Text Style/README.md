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

**To use a font from one of these libraries**, go to the website, select a font and then copy a snippet from the website to import that font from their server into your website. You’ll be given either a `<link>` tag to put in your HTML or an `@import` tag that can be dropped at the top of a CSS file.