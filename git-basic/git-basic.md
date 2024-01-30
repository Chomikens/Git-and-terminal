
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


## Undoing Staged Changes

### `git restore --staged [file name]`

-   **Purpose**: Unstages files that have been added to the staging area, without discarding local changes.
-   **Usage**:
    -   To unstage a specific file, use `git restore --staged [file name]`. This command removes the file from the staging area but keeps the changes in your working directory.
    -   If you accidentally stage a file that you didn't intend to commit, this command is used to revert that action.
-   **Note**: This command does not affect the current changes in the file; it only removes the file from the staging area. The modifications made to the file remain intact in your working directory.

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



## Resetting the Repository

### `git reset --hard [commit]`

-   **Purpose**: Resets the current HEAD, index, and working directory to the state of a specified commit, discarding all local changes.
-   **Usage**:
    -   To reset to a specific commit, use `git reset --hard [commit hash]`.
    -   Without specifying a commit, `git reset --hard` will reset to the latest commit, discarding all changes since then.
-   **Warning**: This command permanently undoes all uncommitted changes and should be used with extreme caution. There is no easy way to recover lost work after using `git reset --hard`.
-   **Common Use Cases**:
    -   Discarding all local changes and returning to the most recent commit state.
    -   Reverting the repository to a known good state if recent commits or changes have introduced issues.