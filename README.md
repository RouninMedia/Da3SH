# Da3SH
*Rich Components for the Web, liberated from JS Frameworks*

## What is Da3SH?

Da3SH is an approach to component-based web architecture in which core web languages (HTML, CSS, Javascript, SVG, PHP etc.) are each serialized as JSON and stored as data.

Whenever needed, each core web language can be unpacked from JSON, on the server-side or on the front-end (client-side).

This liberates the components from JS-first Front-end Reactive Frameworks like ***Angular***, ***React***, ***Vue*** etc.

## The Rise of Component-based Architecture alongside Frameworks

The paradigm of component-based web architecture - which evolved in the 2010s alongside the rise of the giant Front-End Frameworks - has defined its place amongst the schools of web-architecture.

But, being based on Javascript, 2010s-style component-based web architecture evolved with needless baggage, not least the reintroduction of *code-nesting*.

*Code-nesting* refers to web-architecture patterns in which one or more core web languages are nested within a different core web language.

In the late 1990s and early 2000s, the nest-language was HTML:

 - *HTML-inlined JS*
 - *HTML-inlined CSS*

In the 2010s, increasingly, it was Javascript:

 - *JSX (HTML in JS)*
 - *CSS-in-JS*

Whenever core code is nested inside other core code like this - where each uses a syntax radically distinct from the other - the process may result in a large, awkward and unwieldy mixed-mudball of code, in which concerns like *HTML-based structure*, *CSS-based presentation* and *JS-based behaviour* may be difficult to isolate and deal with separately without a suite of task-runners, compilers, transpilers operating at build-time (and sometimes even at runtime).

## Improving on Component-based architecture

The disadvantages of 2010s web-development approaches include:

 - complex toolchain / boilerplate / build setups may be required to even create an environment which make code-nested files possible
 - code-nesting brings everything together, breaking the classic separation of concerns (*structure*, *presentation*, *behaviour*)
 - maintaining something like CSS in JS can quickly become a much larger headache than maintaining a standard, simple CSS stylesheet
 - additionally, future maintenance of dependencies and sub-dependencies (accounting for breaking versions etc.) can quickly become a nightmare (see: https://blog.jim-nielsen.com/2020/cheating-entropy-with-native-web-tech/)

*But*, the advantages of component-based-architecture include:

 - keeping all HTML, JS and CSS code together in a single file (ie. *component-based* separation of concerns) enables portable, re-usable, extensible rich components
 - within components, it's easier to keep track of which classes and data-attributes need to be kept and which may be altered or removed
 - three

## What makes Da3SH different?
In contrast, since it's based on JSON and regards all code as data, Da3SH offers a technology-agnostic alternative to code-within-code.

Da3SH maintains, at all times, a separation between *HTML-based structure*, *CSS-based presentation* and *JS-based behaviour*.

A rich component in Da3SH includes separated "folders" - one for each of these categories - as well as a folder for *SVG-based vector graphics* and another for *JSON-based Data*. Da3SH also allows for named custom subfolders in any of these categories.

By contrast, instead of nesting code-within-code, **Da3SH** treats all code as data.

By employing JSON as a "common data-serialization format", **Da3SH** allows for:

- mono-formatting for code
- single multi-technology files

Most importantly, **Da3SH** retreats from code-nesting and moves back to clean separation of technologies.

**Da3SH** means that a rich web component containing any or all of Markup, Styles, Scripts, Data and even Vectors may be exported as **a consistently-formatted, single file** but **core code remains separated and is never nested within other core code**.

We *can* have the best of both worlds:

 - a website or Single Page App (SPA) divided into separate rich components
 - each rich component divided into fully separated, static (or dynamically-generated) classic concerns:

   - *HTML-based structure*
   - *CSS-based presentation*
   - *JS-based behaviour*
   - *SVG-based vector graphics*
   - *JSON-based data*
