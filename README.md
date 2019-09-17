# Getting Started


## Git Workflow

Projects use a Centralized Workflow meaning that there is a central repository that serves as the single point-of-entry for all changes to the project.

See [here](https://www.atlassian.com/git/tutorials/comparing-workflows) for more information on the centralized workflow.


## Branches
Projects have two permanent branches: `master` and `develop`. The `master` branch contains the most recent stable release. The `develop` branch serves as an integration branch for features.

Temporary `feature` branches can exist which contain features that are being actively developed. Once merged, these feature brances should be deleted. Feature branches have the following naming convention: `feature/feature_name`

## Commit Messages
See [here](https://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html) for commit message guidelines. Commit messages should be short, should be written as commands, and should not have ending punctuation.

Example of a good commit message: `Add readme`

Example of an bad commit message: `Adds readme.`

## Contributing

If this is your first time contributing to the project, clone it. This will create a local version of the repository on your computer.

`git clone https://user@host/path/to/repo.git`

This only needs to be done once for each project you are working on!

Create a new feature branch and push it to the gitlab repository

`git checkout -b feature/feature_name`

`git push -u origin feature/feature_name`

On gitlab, create a new merge request (MR). Append `WIP:` (work in progress) to the beginning of your MR's name. Check the options:
* Delete source branch when merge request is accepted.
* Squash commits when merge request is accepted.

Code and commit your changes

`git add file1 file2`

`git commit -m "Commit message here"`

Push your changes to the gitlab repo

`git push`

If your feature branch is ready, go to your MR and remove the `WIP:` prefix. Then assign it to a teammate for review. If necessary, rebase your MR.