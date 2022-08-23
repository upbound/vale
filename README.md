This repository the home for the Upbound implementation of [Vale](https://vale.sh/).

## What's Vale
Vale is an [open source](https://github.com/errata-ai/vale) command-line tool to provide English language linting. Vale enables spell checking, writing improvements and style guide enforcement in files across text and code.

Vale uses "Packages" to define the set of rules for writing to follow.

## Upbound's use of Vale
Upbound uses the following Vale packages:
- [alex](https://github.com/get-alex/alex) - Catch insensitive, inconsiderate writing. 
- [proselint](https://github.com/errata-ai/proselint) - to try and improve writing styles.
- [Google](https://github.com/errata-ai/Google) - the Google style guide for their Developer Documentation.
- [Microsoft](https://github.com/errata-ai/Microsoft) - based on the Microsoft Writing Style Guide.
- [write-good](https://github.com/errata-ai/write-good) - Naive linter for English prose for developers who can't write good and wanna learn to do other stuff good too.
- [GitLab](https://gitlab.com/gitlab-org/gitlab/-/tree/master/doc/.vale) - The GitLab style guide.
  
Upbound has made some modifications to these packages to remove duplicates or add Upbound specific terms.

## Warnings and errors
Upbound treats warnings and errors the same. All Vale tests must pass for approval.

## Contributing and customizing
Upbound welcomes contributions and changes to the `main` branch. 

Use these guidelines for contributions:
- Edit existing packages first. This includes removing duplicate rules (common with `Google` and `Microsoft`), [adding acronyms](https://github.com/upbound/vale/blob/main/styles/gitlab/Uppercase.yml).
- Add Upbound specific words to the Upbound [Spelling file](https://github.com/upbound/vale/blob/main/styles/Upbound/spelling-exceptions.txt).
- Try to keep any modified lists in a case-insensitive alphabetical order.
