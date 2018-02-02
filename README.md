# vscode-config
common editor config and code style for a project

# setup

-  add to project

    `git submodule add git@github.com:yijie-org/editor-config.git`

    or use https protocol

    `git submodule add https://github.com/yijie-org/editor-config.git`

-  clone a new project with `--recursive` to clone the editor config  submodul

    `git clone --recursive projecrtUrl`

    **ps**: add a `.gitmodules` file in project root directory 

    `.gitmodules` file content like this: 

    ```
    [submodule ".vscode"]
	    path = .vscode
	    url = git@github.com:yijie-org/editor-config.git

    ```

- if clone a new project forget `-recursive` , follow below command

    `git submodule init`

    `git submodule update`

    **ps**: add a `.gitmodules` file in project root directory  

- update submodule to latest commit

    `git submodule update --remote`

- remove submodule

    `git submodule deinit -f .vscode`

    `git rm -rf .gitmodules`

    `git rm -rf .vscode`

- required:

    - `editor config for vscode`

    - `vscode eslint plugin, vscode prettier plugin, vscode solidity plugin`

    - `package.json devDependencies:`

        ```package
            "standard": "^10.0.3",
            "eslint": "^4.10.0",
            "eslint-config-standard": "^10.2.1",
            "eslint-plugin-import": "^2.8.0",
            "eslint-plugin-node": "^5.2.1",
            "eslint-plugin-standard": "^3.0.1"
            "eslint-plugin-react": "^7.5.1"
            "eslint-plugin-promise": "^3.6.0"
        ```
