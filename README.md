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

Whenever core code is nested inside other core code like this - where each uses a syntax radically distinct from the other - the end result may be a large, awkward and unwieldy mixed-mudball of code, in which concerns like *HTML-based structure*, *CSS-based presentation* and *JS-based behaviour* are difficult to isolate and deal with separately without a suite of task-runners, compilers, transpilers operating at build-time (and sometimes even at runtime).

The disadvantages of code-nesting approaches include:

 - complex toolchain / boilerplate / build setups may be required to even create an environment which make code-nested files possible
 - code-nesting brings everything together, breaking the classic separation of concerns (*structure*, *presentation*, *behaviour*)
 - maintaining something like CSS in JS can quickly become a much larger headache than maintaining a standard CSS stylesheet

The advantages of code-nesting include:

 - keeping all HTML, JS and CSS code together in a single file (ie. *component-based* separation of concerns) enables portable, re-usable, extensible rich components
 - within components, it's easier to keep track of which classes and data-attributes need to be kept and which may be altered or removed
 - three

By contrast, instead of nesting code-within-code, **Da3SH** treats all code as data.

By employing JSON as a "common data-serialization format", **Da3SH** allows for:

- mono-formatting for code
- single multi-technology files

Most importantly, **Da3SH** moves away from code-nesting and back to clean separation of technologies.

**Da3SH** means that a rich web component containing any or all of Markup, Styles, Scripts, Data and even Vectors may be exported as **a consistently-formatted, single file** but **core code is never nested within other core code**.

We *can* have the best of both worlds - a website or Single Page App (SPA) divided into separate rich components and each rich component divided into fully separated, static (or dynamically-generated) classic concerns:

 - *HTML-based structure*
 - *CSS-based presentation*
 - *JS-based behaviour*
 - *SVG-based vector graphics*
 - *JSON-based data*
