# CSS Specificity and !important Issues

This repository demonstrates a common problem encountered in CSS: unexpected style application due to specificity conflicts and the overuse of `!important`.  The `bug.css` file shows the problematic code, while `solution.css` provides a more maintainable solution.

## Problem
Specificity in CSS determines which styles are applied when there are multiple conflicting styles.  Inline styles have the highest specificity, followed by internal stylesheets, and then external stylesheets. `!important` further complicates things by overriding any other style.

Overusing `!important` makes the CSS harder to maintain and debug because it makes it very hard to understand what rules are actually being applied.

## Solution
The solution involves carefully considering CSS specificity and avoiding `!important` wherever possible.  This improves the maintainability and predictability of the CSS by making it easier to reason about the style hierarchy.