# actions-list

## GitHub Actions for Code Formatting

This section summarizes the GitHub Actions I commonly use.

### Check dprint Formatting

This action checks the formatting of the code using the `dprint` tool whenever a pull request is made.

- **Name**: Check dprint formatting
- **Trigger**: On pull requests
- **Job**: Runs on the latest version of Ubuntu
- **Steps**:
  1. **Checkout Repository**: Uses `actions/checkout@v2` to check out the repository's code.
  2. **Install dprint**: Installs `dprint` globally using npm.
  3. **Run dprint Check**: Runs the `dprint check` command to verify code formatting.

### Purpose
This action ensures that the code adheres to the formatting rules defined by `dprint`, helping maintain code quality and consistency across the project.
