git-features
============

Git tool to track the merge state of feature branches with environment branches.

## Usage
Ran from within a git repository.

`git features`
Shows the current merge state of features branches to the environment branches.

`git features add <branch> <identifier>`
Add an environment `branch` with a `identifier`.

`git features remove <branch>`
Remove an environment `branch`.

## Example

`git features add staging S`

Adds the staging branch as an environment branch which will be identified by the letter S.

`git features`

Shows the current merge stage of all feature branches (all branches that aren't environment branches; set using `git features add`), in this case all branches apart from staging will show their merge state against the staging branch.

## Installation

Copy the `git-features` script into any directory included in your `PATH`, ensure that `git-features` is executable.
