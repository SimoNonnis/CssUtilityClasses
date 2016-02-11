# CssUtilityClasses
Css (pre/post processor agnostic) utility classes (prefix -u)


Each utility class modifies a single trait.
To apply a trait, or a combination of traits to an element, add the corresponding class directly to the HTML.
Although you won't always want to use combinations of utilities to generate more complicated patterns, the option is there. Refactoring a component's HTML to move particular utility traits into the component's own styles is a relatively simple task.
It has a very specific role (often providing only one declaration) and should
not be bound onto or changed. It can be reused and is not tied to any specific
piece of UI.
It is incredibly important that we signal Utilities to other developers. We do not want anyone trying to bind onto these in future selectors.
Never reassign to anything that carries a leading u-.
Avoid building entire sections of UI out of u-.
Utilities are complete single responsibility rules which have a very specific and targeted task.
Utilities make use of !important, so as to guarantee they beat other less specific ones.
Example use case: using .u-text-center to centrally align one piece of text once and once only.
a utility class like .float-left could show up anywhere, on any element, in any context, so we need to know that it will always do exactly the same thing. That’s why The Authorities agree that utility classes must never change, and why they are a rare case when using !important might be the right choice).
utility classes for straightforward situations calling for very few rules. You just want a button floated right, a centered heading, a different color, invisible text. Why give an element its own name, its own selector, its own ruleset in some stylesheet — why conceptualize a “component” for it — when all you want is to apply a very common, probably very basic pattern?
