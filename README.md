# Try Out Development Containers: Node.js

A **development container** is a running [Docker](https://www.docker.com) container with a well-defined tool/runtime stack and its prerequisites. You can try out development containers with GitHub Codespaces or **[VS Code Remote - Containers](https://aka.ms/vscode-remote/containers)**.

[GitHub Codespaces](https://github.com/features/codespaces) allows you to quickly create customized, cloud-based development environments accessible [from VS Code](https://aka.ms/vso-dl) or the web. 
> **Note:** While GitHub Codespaces is in limited public beta, please _[request access](https://github.com/features/codespaces/signup) if you have not already._

The [VS Code Remote - Containers](https://aka.ms/vscode-remote/download/containers) extension allows you to clone a repository or open any folder mounted into (or already inside) a dev container and take advantage of VS Code's full development feature set. 

This is a sample project that lets you try out either option in a few easy steps. We have a variety of other [vscode-remote-try-*](https://github.com/search?q=org%3Amicrosoft+vscode-remote-try-&type=Repositories) sample projects, too.

> **Note:** If you already have a Codespace or dev container, you can jump to the [Things to try](#things-to-try) section.

## Setting up the development container

### GitHub Codespaces
Follow these steps to open this sample in a Codespace:
1. Click the  Code drop-down menu and select the `Open with Codespaces` option.
  ![image](https://user-images.githubusercontent.com/3174849/103961250-f2cc5e00-5108-11eb-8a15-04a1a2de7491.png)
1. Select `+ New codespace` at the bottom on the pane. This will create a fork of this repository under your account and your codespace will open in a new tab.
   ![image](https://user-images.githubusercontent.com/3174849/103962008-ada92b80-510a-11eb-894d-6e804403acb3.png)
  
### VS Code Remote - Containers
Follow these steps to open this sample in a container using the VS Code Remote - Containers extension:

1. If this is your first time using a development container, please ensure your system meets the pre-reqs (i.e. have Docker installed) in the [getting started steps](https://aka.ms/vscode-remote/containers/getting-started).

2. To use this repository, you can either open the repository in an isolated Docker volume:

    - Press <kbd>F1</kbd> and select the **Remote-Containers: Try a Sample...** command.
    - Choose the "Node" sample, wait for the container to start, and try things out!
        > **Note:** Under the hood, this will use the **Remote-Containers: Clone Repository in Container Volume...** command to clone the source code in a Docker volume instead of the local filesystem. [Volumes](https://docs.docker.com/storage/volumes/) are the preferred mechanism for persisting container data.

    Or open a locally cloned copy of the code:

   - Clone this repository to your local filesystem.
   - Press <kbd>F1</kbd> and select the **Remote-Containers: Open Folder in Container...** command.
   - Select the cloned copy of this folder, wait for the container to start, and try things out!

## Things to try

Once you have this sample opened, you'll be able to work with it like you would locally.

> **Note:** This container runs as a non-root user with sudo access by default. Comment out `"remoteUser": "node"` in `.devcontainer/devcontainer.json` if you'd prefer to run as root.

Some things to try:

1. **Edit:**
   - Open `server.js`
   - Try adding some code and check out the language features. 
   - Notice that `eslint` and the `vscode-eslint` extension are already installed in the container since the `.devcontainer/devcontainer.json` lists `"dbaeumer.vscode-eslint"` as an extension to install automatically when the container is created.
2. **Terminal:** Press <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>\`</kbd> and type `uname` and other Linux commands from the terminal window.
3. **Build, Run, and Debug:**
   - Open `server.js`
   - Add a breakpoint (e.g. on line 20).
   - Press <kbd>F5</kbd> to launch the app in the container.
   - Once the breakpoint is hit, try hovering over variables, examining locals, and more.
   - Continue and from the notification that is shown open a browser. Note you can connect to the server in the container. 
   - The status line shows '1 Port Available'. Clicking the status bar entry shows the 'Ports' view that lists the currently available ports.
4. **Rebuild or update your container** (*Currently, only containers with the VS Code Remote - Containers extension can be rebuilt.*)

   You may want to make changes to your container, such as installing a different version of a software or forwarding a new port. You'll rebuild your container for your changes to take effect. 
   
   **Forward a port statically:** As an example change, let's forward a port statically in the `.devcontainer/devcontainer.json` file. 
     
   > **Note:** Remote-Containers and Codespaces also take care of dynamic port forwarding, but there may be instances in which we want to statically declare a forwarded port. 
   
   - Open the `.devcontainer/devcontainer.json` file.
   - Uncomment the `forwardedPorts` attribute and adjust the port number as needed.
   - Press <kbd>F1</kbd> and select the **Remote-Containers: Rebuild Container** command so the modifications are picked up.

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
