The disadvantages of 2010s web-development approaches include:

 - complex toolchain / boilerplate / build setups may be required to even create an environment which make code-nested files possible
 - code-nesting brings everything together, breaking the classic separation of concerns (*structure*, *presentation*, *behaviour*)
 - maintaining something like CSS in JS can quickly become a much larger headache than maintaining a standard, simple CSS stylesheet
 - additionally, future maintenance of dependencies and sub-dependencies (accounting for breaking versions etc.) can quickly become a nightmare (see: https://blog.jim-nielsen.com/2020/cheating-entropy-with-native-web-tech/)

*But*, the advantages of component-based-architecture which arrived in the 2010s alongside all the above include:

 - keeping all HTML, JS and CSS code together in a single file (ie. *component-based* separation of concerns) enables portable, re-usable, extensible rich components
 - within components, it's easier to keep track of which classes and data-attributes need to be kept and which may be altered or removed
 - three

## What makes Da3SH different?
By contrast, instead of nesting code-within-code as the front-end frameworks do, Da3SH is formatted as JSON and ***regards all code as data***.


By employing JSON as a "common data-serialization format", **Da3SH** allows for:

- mono-formatting for code
- single multi-technology files

Most importantly, **Da3SH** retreats from code-nesting and moves back to clean separation of technologies.

Instead, Da3SH offers code-as-data: a framework-agnostic, language-agnostic alternative to code-within-code.

Consequently,

Da3SH operates simultaneously in two conceptual dimensions:

For the benefit of servers, browsers and technology specialists (the CSS designer who knows little or nothing about Javascript, or the Javascript developer who is unfamiliar with CSS) Da3SH maintains the conventional separation between *HTML-based structure*, *CSS-based presentation* and *JS-based behaviour*.

But, at the same time, for the benefit of web architects, prototypers, project managers and future maintainers, Da3SH *also* groups code by rich component. 

Finally, in contrast to the JS-first frameworks, Da3SH can focus on the HTML-first rather than the JS-first web.

A rich component in Da3SH includes separated "folders" - one for each of these categories - as well as a folder for *SVG-based vector graphics* and another for *JSON-based Data*. Da3SH also allows for named custom subfolders in any of these categories.

**Da3SH** means that a rich web component containing any or all of Markup, Styles, Scripts, Data and even Vectors may be exported as **a consistently-formatted, single file** but **core code remains separated and is never nested within other core code**.
