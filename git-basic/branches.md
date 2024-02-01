# Branches
Branch is a pointer only to the commit!

## Displaying Branches

### `git branch`

-   **Purpose**: Lists all the branches in your repository.
-   **Usage**:
    -   Type `git branch` to see a list of all branches. The current branch will be marked with an asterisk.
    -   Use `git branch -a` to see both local and remote branches.

## Creating Branches

### `git checkout -b [branch-name]`

-   **Purpose**: Creates a new branch and switches to it.
-   **Usage**:
    -   To create and switch to a new branch, use `git checkout -b [branch-name]`.
    -   This is a combination of `git branch [branch-name]` and `git switch [branch-name]`.

### `git branch [branch-name]`

-   **Purpose**: Creates a new branch but does not switch to it.
-   **Usage**:
    -   Type `git branch [branch-name]` to create a new branch without switching to it.
    -   Use `git switch [branch-name]` or `git checkout [branch-name]` to switch to the newly created branch.


## Deleting Branches

### `git branch -d [branch-name]`

-   **Purpose**: Deletes a branch.
-   **Usage**:
    -   To delete a branch, use `git branch -d [branch-name]`.
    -   This command only works if all changes in the branch have been merged into the branch you're currently in. If they haven't, Git will prevent the deletion to avoid losing work.
    -   For force deletion (not recommended unless you are sure), use `git branch -D [branch-name]`.
