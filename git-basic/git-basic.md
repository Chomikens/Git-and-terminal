
# Git Basics

Git is a version control system that allows you to track changes in your source code during software development. Here are some fundamental commands:

## Checking Status and Configurations

### `git status`

-   **Purpose**: Shows the status of files in your Git repository.
-   **Usage**: Type `git status` to see which files are staged, unstaged, or untracked.

## Managing `.gitignore`

### `code .gitignore`

-   **Purpose**: Creates or opens a `.gitignore` file.
-   **Usage**: Type `code .gitignore` to open this file in Visual Studio Code. In this file, list all file patterns that Git should ignore.

## Staging Changes

### `git add .` or `git add [file name]`

-   **Purpose**: Adds files to the staging area.
-   **Usage**:
    -   `git add .` adds all changed files to the staging area.
    -   `git add [file name]` adds a specific file to the staging area.

## Committing Changes

### `git commit -m "[commit message]"`

-   **Purpose**: Records changes to the repository.
-   **Usage**: After staging changes, type `git commit -m "[commit message]"` to commit those changes. The commit message should be a brief description of the changes.

## Viewing Commit History

### `git log`

-   **Purpose**: Shows the commit history.
-   **Usage**: Type `git log` to view the history of commits. It includes the commit ID, author, date, and message.


### `git cat-file`

-   **Purpose**: Provides content or type and size information for repository objects.
-   **Usage**:
    -   To view the content of a Git object (like a commit, tree, or blob), use `git cat-file -p [object hash]`. The `-p` option pretty-prints the object's content.
    -   To get the type of an object (commit, tree, blob), use `git cat-file -t [object hash]`.
    -   To find out the size of an object, use `git cat-file -s [object hash]`.
-   **Example**: To explore a commit, first find its hash using `git log`, then use `git cat-file -p [commit hash]` to view detailed information about the commit.
-   **Note**: This is an advanced command, primarily used for internal inspections and debugging.
