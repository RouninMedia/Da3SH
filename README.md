# Da3SH
*Rich Components liberated from JS Frameworks*

## What is Da3SH?

Da3SH is an approach to web architecture in which core web languages (HTML, CSS, Javascript, SVG, PHP etc.) are all serialized as JSON (and deserialized from JSON).

Being JSON-based, Da3SH offers a technology-agnostic alternative to established web-architecture trends in which one or more core web languages are nested within a different core web language.

In the late 1990s and early 2000s, the nest-language was HTML:

 - *HTML-inlined JS*
 - *HTML-inlined CSS*

In the 2010s, increasingly, it was Javascript:

 - *JSX (HTML in JS)*
 - *CSS-in-JS*

Whenever core code is nested inside other core code like this - where each uses a syntax radically distinct from the other - the end result may be a large, awkward and unwieldy mixed-mudball of code, in which concerns like *structure*, *presentation* and *behaviour* are difficult to isolate and deal with separately.

The disadvantages of historical approaches to code-nesting are:

 - one
 - two
 - three

The advantages - and the reason why code-nesting persists:

 - one
 - two
 - three

By, instead, employing JSON as a "common serialization format", Da3SH allows for:

- mono-formatting for code
- single multi-technology files

Most importantly, **Da3SH** moves away from code-nesting and back to clean separation of technologies.

**Da3SH** means that Markup, Styles, Scripts, Data and even Vectors can be exported simultaneously in **a single file** with consistent formatting, but **core code is never nested within other core code**.
