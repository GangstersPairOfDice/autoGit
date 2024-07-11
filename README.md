# autoGit

Welcome to autogit, a zsh script which automatically inits and pushes a (mostly) empty GitHub repo. All options are optional. If you just run `autogit` by itself, it will init and push a git repo with the current folder name, and the default branch name, using your set GitHub username

## Setup

### 1. Clone this repo and enter the repo's directory

```
git clone https://github.com/GangstersPairOfDice/autoGit.git && cd autoGit
```

### 2. Make the script executable

Run the following command in the terminal to make the script executable:

```
chmod +x autogit
```

If you get errors make sure you are in the same directory as the `autogit` file.

### 3. Update your shell configuration

Add the following line to your shell configuration file (e.g., ~/.zshrc) to update your shell's PATH:

```
export PATH=$PATH:
```

Again, make sure you are in the actual directory where you saved the script.

### 4. Reload your shell configuration

Reload your shell configuration by running:

```
source ~/.zshrc
```

(or `source ~/.bashrc` if you're using Bash)
(NOT TESTED WITH BASH, DIY)

### 5. Verify the setup
Open a new terminal window and type:

```
autogit -h
```

You should see the help message for the autogit script. If you don't see the help message, check that the script is executable and in your system's PATH. That's it You're now ready to use the autogit script to create new Git repositories with ease.

## Usage

```
autogit [options]

  -f <folder_name>: Create a new folder with the specified name and initialize the Git repository inside it.
  -u <github_username>: Set the GitHub username for the remote repository.
  -r <repo_name>: Set the name of the Git repository.
  -b <branch_name>: Set the initial branch name (default: `main`).
  -h: Displays this help menu
```

## Examples


### Initialize a Git repository in the current folder, using the current folders name as the git repo name.

```
autogit
```

### Creates and pushes a new repo into a newly created folder

```
autogit -f newFolder
```

### Creates and pushes a repo with a custom repo name

```
autogit -r myRepo
```

### Create and push a new repository with a custom branch name

```
autogit -b master
```

## Notes

The first time you run this program, if you don't specify the `-u` option, you will be prompted to enter your GitHub username. Subsequent runs will use this username. You can change at any type by specifying the `-u` option.

```
autogit -u <github_username>
```

If you don't specify the `-r` option, the repository name will default to the current folder name.

If you don't specify the `-b` option, the branch name will default to `main`
# autoGit
# autoGit
# autoGit
# autoGit
# autoGit
# autoGit
# autoGit
# autoGit
# autoGit
# autoGit
# autoGit
# autoGit
# autoGit
