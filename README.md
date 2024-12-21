# CSS Specificity Bug

This repository demonstrates a common yet often overlooked issue in CSS: selector specificity. The `bug.css` file contains a CSS rule that unintentionally overrides another due to specificity rules. The `solution.css` file provides a corrected version.

## Bug
The `bug.css` file includes two rules targeting `<p>` elements. The rule `div#container p { color: blue; }` aims to style paragraphs within a specific container differently. However, the more general rule `p { color: red; }` overrides this, causing all paragraphs to be red regardless of their location.

## Solution
The `solution.css` file demonstrates a fix. The specificity of the selector `div#container p` is maintained, ensuring the intended styling is applied.  Alternatively, the order of rules can be adjusted if specificity isn't the issue.