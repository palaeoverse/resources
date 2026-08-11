# Contributing to Palaeoverse

Thanks for stopping by! Looking to find out how you can contribute to **Palaeoverse**? You have come to the right place! 

We very much appreciate and encourage community contributions, and if there is anything that is unclear within this guide, please let us know by logging an [issue](https://github.com/palaeoverse/resources/issues) so we can improve it.

There are multiple ways to contribute to the **Palaeoverse**. This page will go through all of them, starting from the easiest one and progressively increasing the difficulty level.

## Joining the community on Zulip

TODO: add proper link to zulip

TODO: possibly tweak the "anyone can join"

[Zulip]() is where the community gathers to exchange and share useful resources, whether it be papers, job offers, tutorials, or simply to have interesting discussions. Anyone can join this community, and participating there is the easiest way to contribute to the Palaeoverse.

The remaining sections will focus on the software components of the Palaeoverse.

## Participating in existing issues or opening new ones

Tasks that need working on are logged as 'issues' within the respective repository (e.g. current *palaeoverse* issues can be found [here](https://github.com/palaeoverse/palaeoverse/issues)). Participating in the discussion of existing issues or opening new issues for bug reports or feature requests are a great way to start contributing to a package. 

## Contributing to code or documentation

If you want to get involved with contributing some code or documentation to our packages but don't know where to start, you can look for issues labelled 'Good First Issues'. These issues are reserved specifically for new contributors to our packages. Feel free to find one of the unclaimed 'Good First Issues' that interests you, claim it by adding a comment to it, and jump in! Note that you can also work on an issue without this label. 

No matter which issue you want to address, it is good to add a message in the issue to let people know that you are working on it.

### Minor changes

You can fix typos, spelling mistakes, or grammatical errors in the documentation directly on GitHub. 

Note that fixing typos in the function documentation (those in the "Reference" page on the package website) requires editing the source in the corresponding `.R` file and then run `devtools::document()`. *Do not manually edit an `.Rd` file in `man/`*.

### Substantial changes

If you would like to make a substantial change, you should first file an issue and make sure someone from the development team agrees that it’s needed. If you’ve found a bug, please file an issue that illustrates the bug with a reproducible example.

### Contribution workflow (pull request process)

The workflow below requires you to have basic knowledge of git and Github. If this is not the case, you can reach out to one of the [core team members](https://palaeoverse.org/#about-us) via email and they can make a pull request on your behalf. However, you will be expected to respond to any reviewer comments on GitHub (see below).

This describes the process to make a pull request:

1. You (the contributor) should fork the repository (e.g. for the [palaeoverse](https://github.com/palaeoverse/palaeoverse) R package)
1. Clone the desired repository to your personal computer
1. Before changes are made, you should create a new git branch (i.e. not the main branch)
1. Make your changes
1. Commit your changes (make sure your commit message is concise)
1. Push your commits to your forked repository
1. When your changes are complete, you should submit them for merging via a [pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests) (“PR”) on GitHub

Note that a complete pull request should include a succinct description ([see function template](PULL_REQUEST_TEMPLATE.md)) of what the code changes do, proper documentation (via [roxygen2](https://roxygen2.r-lib.org)), and unit tests (via `testthat`). Only the description is required for the initial pull request and code review (see below), but pull requests will not be merged until they contain complete documentation and tests.

You also have to ensure that you follow our [AI policy]().

TODO: add a link to the AI policy


### The life of a pull request

All pull requests must be reviewed by two members of the Palaeoverse ([core team](https://palaeoverse.org/#about-us) before merging. The review process will ensure that contributions 1) meet the standards and expectations as described above, 2) successfully perform the functions that they claim to perform, and 3) don't break any other parts of the codebase.

Submitting a pull request for one of Palaeoverse's R packages will automatically initiate an [R CMD check](https://r-pkgs.org/check.html), [formatting check](https://posit-dev.github.io/air/), [lintr check](https://lintr.r-lib.org/index.html), and [test coverage check](https://covr.r-lib.org/) via GitHub Actions. While these checks will conduct some automatic review to ensure the package has not been broken by the new code and that the code matches the style guide (see above), a manual review is still required before the pull request can be merged.

Reviewers may have questions while reviewing your pull request. You are expected to respond to any of these questions via GitHub. If fixes and/or changes are required, you are expected to make these changes. If the required changes are minor enough, reviewers may make them for you, but this should not be expected. If you have any questions or lack the background to make the required changes, you should work with the reviewer to determine a plan of attack.

## Code review

TODO: This is not the same as addressing the code review of maintainers


## Code of Conduct

Please note that by contributing to **Palaeoverse** you agree to our [Code of Conduct](CODE_OF_CONDUCT.md).
