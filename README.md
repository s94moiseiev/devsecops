# Pre-commit Git Hook with Gitleaks

This is a pre-commit Git hook script that automatically checks for secrets in your code using Gitleaks before allowing a commit. Gitleaks is a tool designed to search for secrets and other sensitive information leaked in a Git repository.

## Installation

1. Copy the `pre-commit` script to your `.git/hooks/` directory in your Git repository.
2. Ensure the script has executable permissions. You can set permissions using `chmod +x pre-commit`.
3. Make sure Gitleaks is installed on your system. You can install it manually or follow the instructions in the script to install it automatically.
4. Optionally, you can enable or disable Gitleaks checks using Git config. To enable, use `git config --add hooks.gitleaks true`. To disable, use `git config --add hooks.gitleaks false`.

## Usage

When you attempt to make a commit, this script will automatically run Gitleaks to check for secrets in your code. If any secrets are found, the commit will be rejected. If no secrets are found, the commit will proceed as usual.

## Dependencies

- Gitleaks: A tool for finding secrets and sensitive information in Git repositories.

## License

This project is licensed under the [MIT License](LICENSE).

## Contribution

Feel free to contribute to the project by opening issues or pull requests on the GitHub repository.

