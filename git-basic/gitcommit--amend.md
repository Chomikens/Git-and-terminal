
# Amending Commits with Git

### `git commit --amend`

-   **Purpose**: Modifies the most recent commit by incorporating new changes, altering the commit message, or both. This command is ideal for correcting minor errors in your last commit, such as forgotten files or typos in the commit message.
    
    ### Modifying the Last Commit
    
    -   **Usage**:
        -   If you've forgotten to include changes in your last commit, stage these changes with `git add` and then run `git commit --amend`. This will open your default commit message editor, allowing you to modify the commit message if needed.
        -   To change the commit message of the most recent commit without altering its content, simply run `git commit --amend` without staging any new changes. This will open the commit message editor with the previous commit message loaded for editing.
    
    ### Options
    
    -   `--no-edit`: Use this option to amend the commit without changing its commit message. Useful when adding forgotten changes to the last commit and you don't want to modify the commit message.
    -   `--author="Author Name <email@example.com>"`: Allows changing the authorship of the commit when amending. This can be useful if you're committing on behalf of someone else or need to correct the author information.
