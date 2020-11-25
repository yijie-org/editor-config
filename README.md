# vscode-config
common editor config and code style for a project

# setup

-  add to project

    `git submodule add git@github.com:yijie-org/vscode-config.git .vscode`

    or use https protocol

    `git submodule add https://github.com/yijie-org/vscode-config.git .vscode`

-  clone a new project with `--recursive` to clone the editor config  submodul

    `git clone --recursive projecrtUrl`

- if clone a new project forget `-recursive` , follow below command

    `git submodule init`

    `git submodule update`

- update submodule to latest commit

    `git submodule update --remote`

- remove submodule

    `git submodule deinit -f .vscode`

    `git rm -rf .gitmodules`

    `git rm -rf .vscode`

- required:

    - `editor config for vscode`

    - `vscode eslint plugin, vscode prettier plugin`

    - `package.json devDependencies:`

      ```shell
      npm install -D --save-exact standard eslint prettier
      ```
