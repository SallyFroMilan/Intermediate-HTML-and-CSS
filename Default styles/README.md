## DEFAULT STYLES

**Browsers**, by default, inject a little bit of style into your web projects, they **insert a little bit of CSS into every webpage**.<br>
The *problem* with this is that there is no guarantee that different browsers will style everything the same. In general, *inconsistencies* are going to be pretty minor, but they DO exist. Also, in many cases as a developer, you’re going to end up *undoing or redoing all of this default styling* to make your site look exactly how you envision it.

To counter this, many developers start their projects with a **“CSS Reset”**(or reset stylesheet): a file that undoes browser defaults, so that **every element behaves the same in every browser**,
is a collection of **CSS rules** used to clear the browser's default formatting of HTML elements, removing potential inconsistencies between different browsers.

The **goal** *of a reset stylesheet* is to reduce browser inconsistencies in things like default line heights, margins and font sizes of headings, and so on.

You don’t have to use a CSS reset. In many cases, you’re going to end up undoing, or redoing a lot of the styles that a reset will provide for you. **You can decide whether or not you want to use one on a regular basis**, but it’s worth taking the time to dig through a couple now. Understanding exactly how they’re doing what they’re doing is a useful exercise!

- **The Meyer Reset** is almost certainly **the most popular**, it basically removes every default style.
- **Normalize.css** is another popular one. It’s a little different in that it doesn’t remove all the default styles, but tweaks them slightly to ensure that browsers are consistent. Significantly different in scope and execution to CSS resets. Is an *alternative to the traditional* CSS reset.