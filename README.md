# autoGit

zsh script which automatically inits and pushes a (mostly) empty git repo.

## Setup

### 1. Save the script

Save the `autogit` script to a directory in your system's PATH, such as `~/bin` or `/usr/local/bin`.

### 2. Make the script executable

Run the following command in the terminal to make the script executable:
```bash
chmod +x ~/bin/autogit

Replace ~/bin/autogit with the actual path to your script file.
3. Update your shell configuration
Add the following line to your shell configuration file (e.g., ~/.zshrc or ~/.bashrc) to update your shell's PATH:

bash
export PATH=$PATH:~/bin

Replace ~/bin with the actual directory where you saved the script.
4. Reload your shell configuration
Reload your shell configuration by running:

bash
source ~/.zshrc

(or source ~/.bashrc if you're using Bash)
5. Verify the setup
Open a new terminal window and type:

autogit -h

You should see the help message for the autogit script. If you don't see the help message, check that the script is executable and in your system's PATH. That's it You're now ready to use the autogit script to create new Git repositories with ease.

## Usage

```
autogit [options]

* `-f, --folder <folder_name>`: Create a new folder with the specified name and initialize the Git repository inside it.
* `-u, --username <github_username>`: Set the GitHub username for the remote repository.
* `-r, --repo <repo_name>`: Set the name of the Git repository.
* `-b, --branch <branch_name>`: Set the initial branch name (default: `main`).

## Examples

### Creates and pushes a new repo into a newly created folder

`autogit -f newFolder`

### Creates and pushes a repo with a custom repo name

`autogit -r myRepo

### Create and push a new repository with a custom branch name

autogit -b master

### Initialize a Git repository in the current folder

autogit

## Notes

The first time you run this program, if you don't specify the `-u` option, you will be prompted to enter your GitHub username. Subsequent runs will use this username. You can change at any type by specifying the `-u` option.

`autogit -u YourGithubUsername`

If you don't specify the `-r` option, the repository name will default to the current folder name.

If you don't specify the `-b` option, the branch name will default to `main`
