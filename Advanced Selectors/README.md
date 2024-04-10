## Advanced CSS selectors and how to target elements in a more specific and finely grained way.
These selectors can be especially useful when you can’t (or don’t want to) change your HTML markup.
There are a lot of advanced selectors, we’ll go through some of the most useful and common ones.

### Child and sibling combinators
Let’s have a look at some more ways we can access different elements *without* referring to their classes. Here are three new selectors to do just that.

(>) - the child combinator<br>
(+) - the adjacent sibling combinator<br>
(~) - the general sibling combinator

To select **all the child and grand-child divs inside of main**, we could write:

    main div {
        /* Our cool CSS */
    }

To select **only the child or grand-child divs** we use the child combinator `>`. Unlike the descendant combinator, it will only select direct children.

    /* This rule will only select divs with a class of child */
    main > div {
        /* Our cool CSS */
    }

    /* This rule will only select divs with a class of grand-child */
    main > div > div {
        /* More cool CSS */
    }

The child selector will select an element that is one level of indentation down. In order to select an element that is adjacent (immediately following) to our target, or on the same level of indentation, we can use the adjacent sibling combinator `+`.

    /* This rule will only select the div with the class child group2 */
    .group1 + div {
        /* Our cool CSS */
    }

    /* This rule will only select the div with the class child group3 */
    .group1 + div + div {
        /* More cool CSS */
    }

Finally, if we want to select **all of the siblings following an element’s** and not just the first one, we can use the general sibling combinator `~`.

    /* This rule will select all of .group1's siblings - in this case the 2nd and 3rd .child divs */
    .group1 ~ div {
        /* Our cool CSS */
    }

Just like the descendant combinator, these selectors *don’t* have any special specificity rules - their specificity score will just be made up of their component parts.

### Pseudo-selectors
**Pseudo-class selectors** are prefixed with a single colon and are a different way to target elements that already exist in HTML.<br>
**Pseudo-elements** are prefixed with two colons and are used to target elements that don’t normally exist in the markup. 

### Pseudo-classes
They offer us different ways to target elements in our HTML. There are quite a lot of them, and they come in a couple of different flavors. Some are based on their position or structure within the HTML. Others are based on the state of a particular element, or how the user is currently interacting with it. Pseudo-classes share the same specificity as regular classes (0, 0, 1, 0). Just like regular classes, most can be chained together.


