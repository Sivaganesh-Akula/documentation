# Config

Command: `git config`

- `--list`: To view all the settings

- `--show-origin`: to view the file system folder where the config is stored

- `--global`: to add the config to the user on the system

- `--local`: to add the config loclly to the repository

- `--system`: to add the config to the system, require admin privileges

## Configs we can add with `--global`, `--local`, `--system`

- `user.name "Siva Ganesh"`: to add name.

- `user.email abc.xyz.com`: to add email id.

- `core.editor app_name`: give the app name or entire path in case of windows. Git specifies the text editor to be used for writing commit messages and other Git-related tasks.
  - `"code --wait"`. The `--wait` flag ensures that Git waits for the editor to close before proceeding.

- `init.defaultBranch`: to modify the default branch
