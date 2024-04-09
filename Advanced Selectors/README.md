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

To select **only the child or grand-child divs** we use the child combinator >. Unlike the descendant combinator, it will only select direct children.

    /* This rule will only select divs with a class of child */
    main > div {
        /* Our cool CSS */
    }

    /* This rule will only select divs with a class of grand-child */
    main > div > div {
        /* More cool CSS */
    }



