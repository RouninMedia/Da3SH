# Da3SH
*Rich Components liberated from JS Frameworks*

**What is Da3SH?**

Da3SH is an approach to web architecture in which core web languages (HTML, CSS, Javascript, SVG, PHP etc.) are all serialized as JSON (and deserialized from JSON).

Being JSON-based, Da3SH provides a technology-agnostic alternative to established JS-first and HTML-first trends in web architecture which contrive to nest one or more core web languages within a different core web language (HTML in the late 1990s and early 2000s; Javascript, increasingly, in the 2010s):

 - HTML-inlined JS
 - HTML-inlined CSS
 - JSX (HTML in JS)
 - CSS-in-JS

Whenever core code is nested inside other core code like this, each using a syntax radically distinct from the other, the end result may be a large, awkward and unwieldy mudball of code, in which concerns like structure, presentation and behaviour are difficult to isolate and deal with separately.

The disadvantages of historical approaches to code-nesting are:

The advantages - and the reason why code-nesting persists -

By employing JSON as a "common serialization format", Da3SH allows for:

- mono-formatting for code
- single multi-technology files

but it does not require code-nesting.
