# CLD

Common Language Documentation

## What?

CLD seeks to provide an extensive, understandable, *common* **documentation** for a variety of programming (and potentially markup, to those "HTML/Markdown/RST is not a language" folk) ***languages***.

## Why?

I had a conversation with a colleague today (2018-12-12) (ISO 8601), and we came upon the following conclusion: the [Python documentation](https://docs.python.org) are intrinsically beautiful <sup>[but not exempt](#do-we-exclude-py)</sup>.

From grammar, to concepts, to standard library example, to standard library internal documentation, it is truly beautiful.

it is *full*. It is *extensive*. It is (mostly) *clear*.

It is formatted in an aesthetically pleasing way. The style itself is aesthetically pleasing as well!

Languages like C, C++, Java, Ruby, Javascript, and more, have one or or more of the following

* expensive documentation
* overly-technical documentation
* for-implementors documentation
* incomplete documentation
* non-official documentation with unfortunate errors or outdated actions
* etc

None of these alone nor combined give either ugly nor beautiful documentation.

Yet the documentation of these languages are objectively *not beautiful*.

Even in the cases that they are beautiful, they contrast from other documentation styles too drastically.

All languages intrinsically share a common syntax.

This is how text editors act on different language code that does the same thing in the same ways-- they form and act upon the [**A**bstract **S**yntax **Tree](https://en.wikipedia.org/wiki/Abstract_syntax_tree).

Therefore, we can solve the problems implicitly declared.

## How?

This serves as a project that will acheive its goal via two major processes:

* documenting abstract language
* documenting specific languages.

The latter includes language examples, and if a standard library exists, the standard library and examples for use.

The latter process also will be done grouped and sorted by language version, recursively, up until the point that the new version is different enough to be considered its own language.

Given any abstract commonality between two languages, it shall be added to the "Abstract Language Syntax" section.

All documentation (at this time) shall be done via Sphinx and/or Mako. It will be published to readthedocs.io under the readthedocs theme. Other themes may also be published, and potentially to other sources. I can't afford much, and intend to do this as a service to anyone without any paywalls nor advertisements (bar advertisements set by the host if the host's model is free hosting and paying for it via ads, like readthedocs).

### Miscellaneous

#### <a id="do-we-exclude-py"></a> Is Python safe?

***No.***

The Python documentation is only beautiful as of 2.5+, or some would even say 3.4+. Even in beauty, there is some ugly. And the Python documentation definitely has some ugly. Plus, it isn't grouped and sorted recursively by version, nor would it ever probably refer to the "Abstract Language Syntax" section.

#### What language will be used for "Abstract Language Syntax"?

None. It shall be done via grammar production lists, and [ootentially interactive] graph diagrams.

#### Will the family of Assembly languages be included?

***Potentially.***

The IA32/64 documentation is several thousand pages long itself. To document any instruction would be documenting it as an *operation*. The documentation for IA32/64 would probably be itself larger than any 3 or 4 other languages combined.

#### Would there be citations?

There will not be any citations to specific pages. At most, there will be [potentially generalized] citation to specific subsections of a document. At worst, there will be [potentially generalized] citations to a document, or in rare cases, no citation at all.

There are aspects historically that truly have *no official source*. If there is a ***widespread** unofficial source*, it shall be cited but noted as unofficial. If there is no widespread source, this documentation has a secondary goal to *become* the widespread unofficial source, and to have the official source revised, appended to, or republished under a new version, with the new information.

If the latter occurs, this document would be upgraded to be the primary, official source for all versions before the republication and here I kindly ask that the republication reference this document for making it aware that the behavior had a standard, yet incorrectly defined or undefined explanation. The republication would be the primary official source for all versions after the republication and this document would become the secondary official source.

If the former two occurs, the citation will be updated to point to the official document and this document will become the secondary, unofficial source.

#### Would there be automation?

Preferably. Especially when it comes to standard library documentation, it would be far better to write a no-op method/structure/object with that language's equivalent of a docstring, and have a tool parse that. Sphinx-Autodoc and Sphinx-Apidoc exist for Python (mostly), but there is minimal alternative tool support for other languages.
