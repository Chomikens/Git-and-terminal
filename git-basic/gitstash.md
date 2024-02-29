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