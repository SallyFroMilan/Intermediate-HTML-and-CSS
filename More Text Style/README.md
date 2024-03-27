## Useful CSS properties that can be used when working with text.

### The system font stack
If you use the `font-family` property to change font and those fonts you are looking for do not happen to be installed on your user’s computer, then a **fallback font** will be displayed. If you have not defined a fallback, then the default HTML font will be used, which is often somewhat ugly. For this reason, it’s common to see somewhat long stacks of fonts listed on projects.

One popular stack is this ‘system font’ stack.

    body {
        font-family: system-ui, "Segoe UI", Roboto, Helvetica, Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
    }

The point of this somewhat ridiculous string of font-families is to try using the default font of the system’s user interface. It will go through each of those fonts until it finds one that is installed on the system, and then use that. Using **a stack like this** often produces *pleasing results*, especially if you’re going for a somewhat *‘neutral’* font style.
