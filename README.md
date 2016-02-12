# CssUtilityClasses
Css (pre/post processor agnostic) utility classes (prefix -u)


Utilities are complete single responsibility rules which have a very specific and targeted task.
They can be reused and are not tied to any specific piece of UI.
**Never reassign to anything that carries a leading u-**, it has a very specific role and should not be bound onto or changed.

A utility class like `.u-textCenter` could show up anywhere, on any element, in any context, so we need to know that it will always do exactly the same thing.

**Utility classes must never change, so they make use of `!important`**.

Why give an element its own name, its own selector, its own ruleset in some stylesheet, why conceptualize a “component” for it, when all you want is to apply a very common, probably very basic pattern?
Utility class names exclusively and transparently represent the styling applied.

Especially for those elements that require only one or two rules and don’t play an obvious role in some component structure, utilities classes should be used.

Further reading: http://davidtheclark.com/on-utility-classes/



###Install (.css)
    cd <path> to folder where you want place the file
    touch utilities.css
    curl https://raw.githubusercontent.com/SimoNonnis/CssUtilityClasses/master/utilities.css > utilities.css

###Install (.scss)
    cd <path> to folder where you want place the file
    touch utilities.scss
    curl https://raw.githubusercontent.com/SimoNonnis/CssUtilityClasses/master/utilities.css > utilities.scss
