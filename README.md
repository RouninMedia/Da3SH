# Da3SH
*Rich Components for the Web. Free from Front-End Frameworks*

## What is Da3SH?

Da3SH is component-based web architecture. But, unlike most other component-based web architecture approaches, Da3SH takes code and encodes it as data.

Da3SH serializes core web languages (HTML, CSS, Javascript, SVG, PHP etc.) as JSON. The serialized snippets are stored together in a single piece of JSON-encoded data representing a single rich component.

Whenever needed, one or more core web language snippets can be unpacked from that single piece of JSON (or Da3SH Module). Since the code is encoded as data, this can happen on the server-side or on the front-end / client-side.

This approach allows different technologies to sit together collectively as components, but - crucially - it liberates those components from *everything-in-JS* Front-end Reactive Frameworks like ***Angular***, ***React***, ***Vue*** etc.

And - despite superficial first appearances - it turns out that *everything-as-JSON* is quite different from *everything-in-JS*.

## Component-based Architecture is good. But it doesn't *need* Frameworks.
Component-based web architecture - which evolved in the 2010s thanks to the rise of the Front-End Reactive Frameworks - has carved out a well-deserved place amongst established web-architecture patterns.

But. As a core feature of the Javascript-first frameworks, 2010s-style component-based web architecture has tended to incorporate excessive, unnecessary baggage.

Most of all: the reintroduction of *code-nesting*.

*Code-nesting* refers to when one or more core web languages are nested within a different core web language.

In the late 1990s and early 2000s, code-nesting was common and the nest-language was HTML:

 - *HTML-inlined JS*
 - *HTML-inlined CSS*

Emphasis on a *Separation of Concerns*, *scalable CSS* and *Unobtrusive Javascript* led to an improved landscape by the late 2000s. 

But in the 2010s code-nesting returned. This time the nest-language was Javascript:

 - *JSX (HTML in JS)*
 - *CSS-in-JS*

There have been attempts to defend the return of code-nesting (mostly by developers who understand Javascript but are less familiar with CSS). One prominent argument is that *Separation of Concerns* is a robust principle but one which makes more sense when the concerns to be separated each represent a *structured, presented, behaviour-oriented Page Component* rather than one of the technologies declaring structure, presentation or enabling behaviour across the entire live web document.

From an overview perspective, there is something in this. But the fact remains: whenever core code is nested inside other core code like this - where each uses a syntax radically distinct from the other - the process may result in a large, awkward, not-easily-separable mixed-mudball of code, in which concerns like *HTML-based structure*, *CSS-based presentation* and *JS-based behaviour* may be difficult to isolate and refactor separately without a suite of task-runners, compilers, transpilers etc. operating at build-time (and sometimes even at runtime).

Even HTML 3.2 (from 1996) is better than this. Because, while it mashes structure and presentation together, it does so using only one syntax:

    <BODY BGCOLOR="#FFFFFF">
     <CENTER>
      <H1>This is HTML 3.2</H1>
      <P>It handles presentation without CSS.</P>
     </CENTER>
    </BODY>
    
And, in any case, who said we had to have one or the other? Why can't a page be separated into page components and each page component be separated into technologies. That's not going to be possible, of course, if every page component consists exclusively of javascript. But in Da3SH, rich components aren't made out of javascript - they're just JSON-formatted data.  

## Improving on 2010s-style Component-based architecture
Outside building complex web-apps, frameworks usually represent exasperating over-engineering.

But there's no need to throw the baby out with the bathwater: reusable, customisable components remain entirely useful in the context of building a conventional website no less than in a 100% JS Single Page Application (SPA).

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

We *can* have the best of both worlds:

 - a website or Single Page App (SPA) divided into separate rich components
 - each rich component divided into fully separated, static (or dynamically-generated) classic concerns:

   - *HTML-based structure*
   - *CSS-based presentation*
   - *JS-based behaviour*
   - *SVG-based vector graphics*
   - *JSON-based data*

What if *all* we want is a plain and simple HTML + CSS website with an occasional slice of JS to enable interactivity... *but* in building that website we want to be able to deploy shareable, reusable, easy-to-modify but pre-constructed building blocks within that environment-of-simplicity?

That's **Da3SH**.

## Don't WebComponents already exist?
WebComponents *do* exist but the difference between **WebComponents** and **Da3SH Modules** is that the former are intended to represent re-usable *primitive components*, while the latter represent re-usable *rich components*. Further, WebComponents will not work in javascript-disabled browsers, whereas, if required, framework-agnostic, language-agnostic **Da3SH** allows developers to build javascript-free websites.
