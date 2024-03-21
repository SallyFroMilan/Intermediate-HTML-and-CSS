## CSS values and units
CSS rules contain declarations, which in turn are composed of properties and values. Each property used in CSS has a **value type** that describes what kind of values it is allowed to have.

### What is a CSS value?
**Value types** are surrounded by angle brackets, such as `<color>` or `<length>`. For example, when you see the value type `<color>` as valid for a particular property means you can use any valid color as a value for that property, as listed on the `<color>` reference page.

### Lengths
The **numeric type** you will come across *most frequently* is `<length>`. There are two types of lengths used in CSS, part of the **CSS Units**: **relative and absolute**.

### CSS Units
There are many different units that you can use to **define sizes in CSS**, the most important are **relative and absolute units**.

### Absolute length units
are those that are **always the same in any context**.<br>
`px` is an absolute unit because *the size of a pixel doesn’t change* relative to anything else on the page. In fact, `px` **is the only absolute unit you should be using for web projects**. The rest of them make more sense in a print setting because they are related to physical units such as `in` (inch) and `cm` (centimeter) - we don't typically use cm on screen.

### Relative length units
are units that **can change based on their context**.<br>
Are relative to something else, perhaps the size of the parent element's font, or the size of the viewport. The **benefit** of using relative units is that with some careful planning you can make it so the size of text or other elements scales relative to everything else on the page. There are several of them that you are likely to encounter and want to use.

### em and rem
`em` and `rem` both refer to a **font size**, though *they are often used* to **define other sizes in CSS**. You’ll see both of them often so we’re going to explain both, but as a rule-of-thumb, **prefer `rem`**.

`1em` is the `font-size` of an **element** (**or the element’s parent** if you’re using it to set `font-size`). So, for example, if an element’s `font-size` is `16px`, then setting its width to `4em` would make its width `64px` (`16 * 4 == 64`).

`1rem` is the `font-size` of the **root element** (either `:root` or `html`). The math works the same with `rem` as it did with `em`, but without the added complexity of keeping track of the parent’s font size. Relying on `em` could mean that a particular size could change if the context changes, which is very likely not the behavior you want.

Using a relative size like `rem` to define font sizes across your website is recommended. Many browsers allow users to change the base font-size to increase readability. If at all possible, it is advisable to respect a user’s wishes regarding font size. You’ll learn more about this from the reading assignments.

### Viewport units
The units `vh` and `vw` relate to the size of the viewport. Specifically, `1vh` is equal to `1%` of the viewport height and `1vw` is equal to `1%` of the viewport width. These can be useful any time you want something to be sized relative to the viewport, examples including full-height heroes, full-screen app-like interfaces.
