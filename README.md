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
