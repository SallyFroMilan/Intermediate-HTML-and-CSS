## HTML TABLES
allow you to create **two-dimensional tables made of rows and columns**. 

Some data just *really needs to be displayed* in a **table**. **HTML tables** might be *less commonly used* than buttons, links, lists and everything else you’ve learned so far, but there are **some cases where they’re the perfect tool**.

Some of the more advanced features can get a little tricky to set up correctly but getting started with tables is pretty easy. You create a table with `<table></table>` tags and then put the elements for rows, columns, headers, or anything else that’s possible inside those table elements.

For **tables, to be effective on the web**, you need to provide some styling information with CSS, as well as good solid structure with HTML.

## When should you NOT use HTML tables?

**HTML tables should be used for tabular data** — this is what they are designed for.<br> Unfortunately, a lot of people used to use HTML tables to lay out web pages, e.g. one row to contain the header, one row to contain the content columns, one row to contain the footer, etc. This was commonly used because CSS support across browsers used to be terrible; table layouts are much less common nowadays, but you might still see them in some corners of the web.

    In short, using tables for layout rather than CSS layout techniques is a bad idea.

The **main reasons** are:

- **Layout tables reduce accessibility for visually impaired users:** screen readers, used by blind people, interpret the tags that exist in an HTML page and read out the contents to the user. **Table markup is** *more complex* than with CSS layout techniques so the screen readers' output will be confusing to their users.
- **Tables produce tag soup:** as mentioned above, table layouts generally involve more complex markup structures than proper layout techniques. This can result in the code being harder to write, maintain, and debug.
- **Tables are not automatically responsive:** when you use proper layout containers (such as `<header>`, `<section>`, `<article>`, or `<div>`), their width defaults to 100% of their parent element. Tables on the other hand are sized according to their content by default, so extra measures are needed to get table layout styling to effectively work across a variety of devices.