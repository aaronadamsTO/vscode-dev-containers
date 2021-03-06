# Python 3 - Miniconda

## Summary

*Develop Python 3 - Miniconda applications. Installs dependencies from your environment.yml file and the Python extension.*

| Metadata | Value |  
|----------|-------|
| *Contributors* | The [VS Code Python extension](https://marketplace.visualstudio.com/itemdetails?itemName=ms-python.python) team |
| *Definition type* | Dockerfile |
| *Languages, platforms* | Python |

## Using this definition with an existing folder

First, for convenience, this definition will automatically install dependencies from your `environment.yml` file when the container is built. However, note that `environment.yml` in the root of this definition folder is **only present for testing** and is not used or required by the definition itself.

Second, only the integrated terminal is supported by the Remote - Containers extension. You may need to modify `launch.json` configurations to include the following value if an external console is used.

```json
"console": "integratedTerminal"
```

Beyond that, just follow these steps:

1. If this is your first time using a development container, please follow the [getting started steps](https://aka.ms/vscode-remote/containers/getting-started) to set up your machine.

2. To use VS Code's copy of this definition:
   1. Start VS Code and open your project folder.
   2. Press <kbd>F1</kbd> select and **Remote-Containers: Add Development Container Configuration Files...** from the command palette.
   3. Select the Python 3 - Miniconda definition.

3. To use latest-and-greatest copy of this definition from the repository:
   1. Clone this repository.
   2. Copy the contents of `containers/python-3-miniconda/.devcontainer` to the root of your project folder.
   3. Start VS Code and open your project folder.

4. After following step 2 or 3, the *only* the contents of the `.devcontainer` folder in your project can be adapted to meet your needs. Ignore other files and folders.

5. Finally, press <kbd>F1</kbd> and run **Remote-Containers: Reopen Folder in Container** to start using the definition.

## Testing the definition

This definition includes some test code that will help you verify it is working as expected on your system. Follow these steps:

1. If this is your first time using a development container, please follow the [getting started steps](https://aka.ms/vscode-remote/containers/getting-started) to set up your machine.
2. Clone this repository.
3. Start VS Code, press <kbd>F1</kbd>, and select **Remote-Containers: Open Folder in Container...**
4. Select the `containers/python-3-miniconda` folder.
5. After the folder has opened in the container, press <kbd>F5</kbd> to start the project.
6. A `test-project/plot.png` file should be added to the folder after it runs with the plot result.
7. Next, open `test-project/hello.py` and press <kbd>ctrl/cmd</kbd>+<kbd>a</kbd> then <kbd>shift</kbd>+<kbd>enter</kbd>.
8. You should see the `matplotlib` output in the interactive window.
9. From here, you can add breakpoints or edit the contents of the `test-project` folder to do further testing.

## License

Copyright (c) Microsoft Corporation. All rights reserved.

Licensed under the MIT License. See [LICENSE](https://github.com/Microsoft/vscode-dev-containers/blob/master/LICENSE)
