# Try Out Development Containers: Node.js

This is a sample project to go along with the "try" quick start for the **[VS Code Remote - Containers](https://aka.ms/vscode-remote/containers)** extension.

**If you aren't already following the quick start, [see here](#setting-up-the-development-container).**

## Things to try

One you have this sample opened in a container, you'll be able to work with it like you would locally.

Some things to try:

1. **Use a Terminal to install needed dependencies:**
   1. Press <kbd>ctrl</kbd>+<kbd>shift</kbd>+<kbd>\`</kbd> to open a terminal window
   2. Type `yarn install`
   3. The command will run even if you don't have yarn installed locally!
2. **Edit:**
   1. Open `server.js`
   2. Try adding some code and check out the language features.
3. **Build, Run, and Debug:**
   1. Open `sever.js`
   2. Add a breakpoint.
   3. Press <kbd>F5</kbd> to launch the app in the container.
   4. Once the breakpoint is hit, try hovering over variables, examining locals, and more.
   5. Continue, then open a local browser and go to `http://localhost:3000` and note you can connect to the server in the container.
4. **Forward another port:**
   1. Stop debugging
   2. Open `sever.js`
   3. Change the server port to 5000. (`const PORT = 5000;`)
   4. Press <kbd>F5</kbd> to launch the app in the container.
   5. Press <kbd>F1</kbd> and run the **Remote-Containers: Forward Port...** command.
   6. Select port 5000.
   7. Click "Open Browser" in the notification that appears to access the web app on this new port.

## Setting up the development container

Follow these steps to open this sample in a container:

1. If this is your first time using a development container, please follow the [getting started steps](https://aka.ms/vscode-remote/containers/getting-started) to get set up.

2. If you're not yet in a development container:
   1. Clone this repository.
   2. Press <kbd>F1</kbd> and select the **Remote-Container: Open Folder in Container...** command.
   3. Select the cloned copy of this folder, wait for the container to start, and try things out!


3. **[Windows]** Disable automatic line ending conversion for Git on the *Windows side* (given Linux and Windows use different line endings). Run: `git config --global core.autocrlf false`
4. Follow the steps at [https://aka.ms/vscode-remote/containers/getting-started](https://aka.ms/vscode-remote/containers/getting-started).
5. Run `yarn install`
6. Launch the application, edit, and try things out!


## Contributing

This project welcomes contributions and suggestions.  Most contributions require you to agree to a
Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
the rights to use your contribution. For details, visit https://cla.microsoft.com.

When you submit a pull request, a CLA-bot will automatically determine whether you need to provide
a CLA and decorate the PR appropriately (e.g., label, comment). Simply follow the instructions
provided by the bot. You will only need to do this once across all repos using our CLA.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.

## License

Copyright © Microsoft Corporation All rights reserved.<br />
Licensed under the MIT License. See LICENSE in the project root for license information.
