# Uncommon HTML Bug: Unexpected InnerHTML Behavior

This repository demonstrates a subtle bug related to using `innerHTML` to modify the content of a div element in HTML.

The `bug.html` file shows the incorrect way to append content, and `bugSolution.html` shows how to fix it.

The problem arises when using `+=` with `innerHTML` on a div containing multiple child nodes.  Instead of correctly appending, it can overwrite the original content in unexpected ways. This behavior is not immediately obvious and can cause frustrating debugging sessions.

The solution involves using `insertAdjacentHTML` for safer and more predictable content insertion.