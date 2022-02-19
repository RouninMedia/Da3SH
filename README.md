# DaNIS³H
*Rich Components for the Web. Free from Front-End Frameworks.*

## What is DaNIS³H?

**DaNIS³H** (***D**ata **a**nd **N**atively **I**mportable **S**tyles, **S**cripts, **S**VG & **H**TML*) is an approach which enables component-based web architecture even outside JS-frameworks.

Unlike most other component-based approaches to web-architecture, **DaNIS³H** takes code and encodes it as *data*.

This means **DaNIS³H** can be framework free.

To use **DaNIS³H**, you don't need to spend weeks (or months) learning a framework and then discover in 3-4 years time that that's *all "old" now* and you have to repeat the process with a new, shiny framework.

***DaNIS³H** essentially does away with frameworks.*

You can write standard HTML, CSS, JavaScript, SVG (whatever...) and **DaNIS³H** will give you back a single-file encapsulated module which you can then deploy on any website with a **DaNIS³H** interpreter.

**DaNIS³H** serializes core web languages (HTML, CSS, Javascript, SVG, PHP etc.) as JSON. The serialized snippets are combined and stored together as a single piece of JSON-encoded data representing a single rich component.

Then, whenever needed, one or more core web language snippets can be unpacked from that single piece of JSON (or **DaNIS³H Capsule**). Since the code within the capsule is encoded as *data*, *any* scripting language on the server-side *or* on the front-end / client-side can perform the unpacking.

This approach allows different front-end technologies to sit together collectively to represent a self-contained front-end component, but in such a way that the component is liberated from *everything-in-JS* Front-end Reactive Frameworks like ***Angular***, ***React***, ***Vue*** etc.

And - despite expectations - it turns out that *everything-as-JSON* is quite different from *everything-in-JS*.

## Deploying Reusable Components is a smart approach to Web Architecture 
*But it's even smarter when it's no longer tied to a single scripting language.*

Component-based web architecture - which evolved in the 2010s thanks to the rise of the Front-End Reactive Frameworks - has carved out a well-deserved place amongst established web-architecture patterns.

But. As a core element of those JS-first frameworks, 2010s-style component-based web architecture heralded the unwelcome return of *code-nesting*. Core web languages (HTML, CSS, JS, SVG) are inter-dependent but they have radically different syntaxes, handle separate responsibilities and live (conventionally) in separate files. Often they are developed by different professionals. They are *meant* to be separated.

*Code-nesting* refers to when one or more core web languages are nested within a different core web language.

In the late 1990s and early 2000s, code-nesting was common and the nest-language was HTML:

 - *HTML-inlined JS*
 - *HTML-inlined CSS*

Emphasis on a *Separation of Concerns*, *scalable CSS* and *Unobtrusive Javascript* led to an improved landscape by the late 2000s. Semantic HTML Architects, CSS Designers and Javascript Engineers were each able to focus on their disciplines unhindered by external code.

But in the 2010s code-nesting returned. This time the nest-language was Javascript:

 - *JSX (HTML in JS)*
 - *CSS-in-JS*

There have been attempts to defend the return of code-nesting (mostly by developers who understand Javascript but can be dismissive of HTML and remain unfamiliar with CSS).

One prominent argument is that *Separation of Concerns* is a robust principle but one which makes more sense when the concerns to be separated each represent a *structured, presented, behaviour-oriented Page Component* rather than one of the technologies declaring structure, declaring presentation or enabling behaviour across the entire live web document.

From an overview perspective, there *is* something in this. But the fact remains: whenever core code is nested inside other core code - and each respective language uses a syntax radically distinct from the other - the process may result in a large, unwieldy, not-easily-separable mixed-mudball of code, in which concerns like:

 - *HTML-based structure*
 - *CSS-based presentation*
 - *JS-based behaviour*

may be difficult to isolate and refactor separately without a suite of task-runners, compilers, transpilers etc. operating at build-time (and sometimes even at runtime).

Arguably, even HTML 3.2 (from 1996) is better than this. Because, while it mashes structure and presentation together, it does so using only one syntax:

    <BODY BGCOLOR="#FFFFFF">
     <CENTER>
      <H1>This is HTML 3.2</H1>
      <P>It handles presentation without CSS.</P>
     </CENTER>
    </BODY>
    
And, in any case, who said we had to have one type of separation or the other?

Why can't a page be separated into page components *and* each page component be separated into technologies? 

That's not going to be possible, of course, *if* every page component is built exclusively out of javascript.

But in **DaNIS³H**, rich components *aren't* made out of javascript - they're simply JSON-formatted *data*.

That data can be translated *by* any scripting language (JS, PHP, Python, Ruby etc.) *into* whichever language is intended as the target (HTML, CSS, JS, SVG etc.).

## Improving on 2010s-style Component-based architecture
Reactive front-end frameworks are hugely complex. Outside building sophisticated web-apps, such frameworks can represent an exasperating level of over-engineering.

But there's no need to throw the baby out with the bathwater. Web-developers shouldn't have to choose between frameworks-including-components and no-components-at-all.

Reusable, customisable components remain entirely useful when building *a conventional content-based website* no less than when building an exclusively JS-based Single Page Application (SPA).

**DaNIS³H** allows developers to write and deploy rich components without using or installing a framework at all.

We *can* have the best of both worlds:

 - a website or Single Page App (SPA) divided into separate rich components
 - each rich component divided into fully separated, static (or dynamically-generated) language-based concerns:

   - *HTML-based structure*
   - *CSS-based presentation*
   - *JS-based behaviour*
   - *SVG-based vector graphics*
   - *JSON-based data*

What if *all* we want is a plain and simple HTML + CSS website with an occasional slice of JS to enable interactivity...

... *but* in building that website we want to be able to deploy shareable, reusable, easy-to-modify but pre-constructed building blocks within that zero-build-process environment-of-simplicity?

That's **DaNIS³H**.

______

## Wait a second... don't native WebComponents already exist?
Yes. Since late 2018, cross-browser-compatible, native **WebComponents** *do* exist.

The difference between native **WebComponents** and native-like **DaNIS³H Modules** is that the former were designed to represent re-usable *primitive components*, while the latter represent re-usable *rich components*.

*For an eloquent and articulate discussion regarding the importance of primitive components, see:*

 - <a href="https://lea.verou.me/2020/09/the-failed-promise-of-web-components/" title="The Failed Promise of WebComponents by Lea Verou" target="_blank">https://lea.verou.me/2020/09/the-failed-promise-of-web-components/</a>.

Apart from anything else, **WebComponents** will *not* work in javascript-disabled browsers.

In huge contrast, **DaNIS³H** - being framework-agnostic, library-agnostic, language-agnostic - allows developers to build from components websites which are entirely javascript-free .
