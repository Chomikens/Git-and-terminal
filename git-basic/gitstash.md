# Stashing Changes

### `git stash`

-   **Purpose**: Temporarily saves changes in your working directory and index, allowing you to work on something else or switch branches without committing unfinished changes.
-   **Usage**:
    -   Type `git stash` to stash changes in your working directory and index.
    -   This command is useful when you need to switch branches or perform other tasks without committing changes.
    -   Stashing does not affect the committed history of your repository.

    ### `git stash list`

-   **Purpose**: Lists all stashed changes.
-   **Usage**: Type `git stash list` to see a list of all stashed changes.
-   The list includes a stash reference (e.g., `stash@{0}`), along with a description of the stashed changes and the commit where the stash was created.

### `git stash apply [stash reference]`

-   **Purpose**: Applies the changes from a specific stash to your working directory and index without removing it from the stash list.
-   **Usage**:
    -   Type `git stash apply [stash reference]` to apply the changes from a specific stash.
    -   You can use `git stash list` to find the reference of the stash you want to apply.

### `git stash pop [stash reference]`

-   **Purpose**: Applies the changes from a specific stash to your working directory and index and removes it from the stash list.
-   **Usage**:
    -   Type `git stash pop [stash reference]` to apply the changes from a specific stash and remove it from the stash list.
    -   Similar to `git stash apply`, but removes the applied stash from the list after applying.

### `git stash drop [stash reference]`

-   **Purpose**: Removes a specific stash from the stash list.
-   **Usage**:
    -   Type `git stash drop [stash reference]` to remove a specific stash from the stash list.
    -   Useful for cleaning up the stash list after applying or resolving stashed changes.

### `git stash clear`

-   **Purpose**: Removes all stashed changes from the stash list.
-   **Usage**: Type `git stash clear` to remove all stashed changes from the stash list.
-   Useful for clearing out old or unnecessary stashes, especially after they have been applied or resolved.

### `git stash show [stash reference]`

-   **Purpose**: Displays the changes stored in a specific stash.
-   **Usage**:
    -   Type `git stash show [stash reference]` to display the changes stored in a specific stash.
    -   Shows a summary of the changes, including file names and a brief overview of modifications.

### `git stash branch [branch name] [stash reference]`

-   **Purpose**: Creates a new branch from a specific stash and applies the changes to that branch.
-   **Usage**:
    -   Type `git stash branch [branch name] [stash reference]` to create a new branch from a specific stash and apply the changes to that branch.
    -   Useful for working on stashed changes in isolation, without affecting the current branch.