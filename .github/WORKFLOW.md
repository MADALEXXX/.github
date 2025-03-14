# Workflow
This is extended from 
[CONTRIBUTING.md](https://github.com/MADALEXXX/.github/blob/main/.github/CONTRIBUTING.md).
Please read that document before perusing this one, as it provides a general
overview of the workflow and additional guidelines.

This workflow is a loose adaptation of a [Trunk-Based Development][trunkdev] workflow.
this emphasizes forks and individual or small team contributions from forks.

# Git branches

There is one major branch:

1. main

-   This branch is protected
-   GitHub Actions run on pull request submissions
-   Pull request approvals are required before they are merged
-   This contains production ready code
-   This is code that users are using
-   Possible impact to users' apps if something goes wrong
-   New commit triggers auto deployment where applicable

There are a number of naming conventions for development branches you'll work
on in your fork:

1. [username]/feature/[feature-name]

-   New feature based on issue or request
-   This branch is created from your fork's `main` branch
-   This can be deleted

4. [username]/patch/[feature]

-   Used to patch new features that are almost ready for submission or
    whose submission has been closed due to a number of fixes that need
    to be implemented

5. hotfix/x.x.x

-   Ideally, this will be used sparingly
-   In case a bug is found in production, this is to prioritize review
-   Very small changes should be made in these branches, specifically to
    address bugs in production and nothing else
-   Should be merged quickly upon approval

## Contributor workflow

### Fork repository

### Create feature branch from main

### Create PR from my-username/feature/my-new-feature -> main

-   PR is reviewed,
-   Review confirms it works, follows contribution conventions, looks good
-   Developer test PR in local computer, their discord server
-   CI/CD will validate that all test cases are good
-   PR reviewers test cases are created
-   CI/CD will validate tests and verify code adheres to guidelines
-   Deploy to test linux/ubuntu server
-   Deploy to shared test guild
-   CI/CD integration validation

### PR merged to main

-   Production release
-   Have a call with devs to ensure everything runs smoothly

And remember to Document, Document, Document!

<!--link dump-->
[trunkdev]: https://trunkbaseddevelopment.com