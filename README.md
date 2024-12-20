# PHP Session Error: Output Before session_start()

This repository demonstrates a common error in PHP related to session handling.  The error occurs when output is sent to the browser *before* the `session_start()` function is called.  This can lead to unexpected behavior and prevent sessions from functioning correctly.

The `bug.php` file showcases the erroneous code, while `bugSolution.php` provides the corrected version.

**How to reproduce:**
1. Run `bug.php`.
2. Observe the error or unexpected behavior.
3. Run `bugSolution.php` to see the corrected behavior.

This example highlights the importance of calling `session_start()` before any other output is sent to the client. This includes whitespace, HTML tags, or any other data that might be sent to the browser.