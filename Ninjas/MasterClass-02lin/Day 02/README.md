# Day 02 Notes


# 1. **Understanding GitHub Workflow**
The GitHub workflow includes the complete process from starting to submitting code and merging. Here is the standard process:

## Steps:
- **Fork the repository**: Copy the main repository (original repository) to your own GitHub account and create your development branch.
  
  
- **Clone the repository**: Clone the forked repository to your local machine for code editing.
  
- **Edit the code**: Make changes to the code locally, preparing it for submission.

- **Commit changes**: Use Git commands to commit the changes to the local repository and push them to the branch on GitHub.
  - Steps:
    1. In VS Code, select the branch.
    2. Open Git Bash terminal and execute:
        - `git add .` to add the modified files.
        - `git commit -m "description text"` to commit changes with a meaningful description.
        - `git push` to push the changes to the branch on GitHub.
 

- **Create a Pull Request (PR)**: On GitHub, create a PR to request merging your changes into the main repository's main branch.


- **PR Approval and Merge**: The repository owner (typically a senior developer) approves the PR and merges it.

- **Synchronize the main repository**: After the merge, ensure that both local and remote repositories are synchronized with the main repository, updating all branches in the codebase.


---

# 2. **Understanding Markdown Syntax**
Markdown is a simple text formatting language used to write formatted text. It is commonly used for README files and documentation.

## Common Markdown Syntax:
- **Headings**: Use `#` to create headings of different levels, e.g., `# H1`, `## H2`, etc.
- **Lists**: Use `-` or `*` for unordered lists and `1.` for ordered lists.
- **Links**: `[Link Text](URL)` format.
- **Code blocks**: Use backticks `` `code` `` for inline code, and three backticks ``` for multi-line code.
- **Text Styles**: Use `**bold text**` and `*italic text*`.

---

# 3. **Adding the Markdown Preview Github Styling Plugin in VS Code**
To preview Markdown content in VS Code, you can install the **Markdown Preview Github Styling** plugin. Follow these steps:

1. **Open VS Code**.
2. **Open the Extensions View**: Press `Ctrl+Shift+X`.
3. **Search for the Plugin**: In the search bar, type `Markdown Preview Github Styling`, find the plugin, and install it.
4. **Preview Markdown**: Once installed, use the preview feature to view the formatted Markdown content, similar to how it appears on GitHub.




| Day   | Date       | Hours | Time Period  | Topic                      |
|-------|------------|-------|--------------|----------------------------|
| Day 2 | 2024-12-14 | 2     | 19:30 - 21:30 | Markdown and Git add, push |
