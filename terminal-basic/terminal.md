
# Terminal Basics

## Navigating Directories

### `pwd`

-   **Purpose**: Displays the current directory path.
-   **Usage**: Type `pwd` to see the full path of the directory you're currently in.

### `ls`

-   **Purpose**: Lists all files and directories in the current directory.
-   **Usage**: Type `ls` for a basic list. Use `ls -l` for detailed information, or `ls -a` to include hidden files.

### `cd [directory]`

-   **Purpose**: Changes the current directory.
-   **Usage**: Type `cd [directory name/path]` to move to a specified directory. Use `cd ..` to go up one level. `cd` without arguments takes you to the home directory.

## Managing Files and Directories

### `mkdir [directory name]`

-   **Purpose**: Creates a new directory.
-   **Usage**: Type `mkdir [directory name]` to create a new directory in the current location.

### `touch [file name]`

-   **Purpose**: Creates a new file.
-   **Usage**: Type `touch [file name]` to create a new file in the current directory.

### `rm [file name]`

-   **Purpose**: Removes a file.
-   **Usage**: Type `rm [file name]` to delete a file. Use caution as this cannot be undone.

### `rm -r [directory name]`

-   **Purpose**: Removes a directory and its contents.
-   **Usage**: Type `rm -r [directory name]` to delete a directory and all files within it.

### `cat [file name]`

-   **Purpose**: Displays the content of a file or files.
-   **Usage**:
    -   To view the contents of a file, type `cat [file name]`.
    -   To concatenate two or more files, type `cat file1 file2 > combinedfile`.
    -   To add content to a file, type `cat >> [file name]`, then enter the content and press `CTRL+D` to save.
    -   Useful for quickly viewing or combining small files.

## Additional Commands

### `code [file name]`

-   **Purpose**: Opens a file in Visual Studio Code.
-   **Usage**: Type `code [file name]` to open or create a file in VS Code. If the file doesn't exist, this command will create it.

### Tips for Using Terminal

-   **Autocomplete**: Press `Tab` to autocomplete file or directory names.
-   **History**: Use the `up` and `down` arrow keys to cycle through previously used commands.
-   **Clear Screen**: Type `clear` to clean up the terminal view.
