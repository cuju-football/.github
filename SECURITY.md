# Security

Cuju runs code that other people write. The renderer and the arena load submissions, start their processes and read their files, so a flaw in how they do that matters to everyone who runs a tournament or a shared evaluation.

## Reporting a vulnerability

Report a vulnerability privately through the repository it affects, with the Report a vulnerability button under its Security tab. That keeps the report between you and the maintainers until a fix is out. Include the package and its version, what you did, what happened, and what you expected, with a small example where you can.

Reports are answered as soon as the maintainers can, and a fix is released for the latest version of each package. Once it is out, the advisory is published with credit to the reporter, unless they ask to stay unnamed.

## What counts

Anything that lets a submission, a recording, a team folder or a format escape the limits the packages promise counts, such as reading or writing outside its folder, outliving its match, passing a safety ceiling unnoticed, or running code when a file is only opened. A result that differs from Google Research Football is a bug rather than a vulnerability, and belongs in the issues.
