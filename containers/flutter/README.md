# Flutter

## Summary

*Develop Flutter based applications. Includes the Flutter SDK, needed extensions, and dependencies.*

| Metadata | Value |  
|----------|-------|
| *Contributors* | @anTup |
| *Definition type* | Dockerfile |
| *Languages, platforms* | Flutter/Dart |

## Using this definition with an existing folder

This definition does not require any special steps to use. Just follow these steps:

1. If this is your first time using a development container, please follow the [getting started steps](https://aka.ms/vscode-remote/containers/getting-started) to set up your machine.

2. To use VS Code's copy of this definition:
   1. Start VS Code and open your project folder.
   2. Press <kbd>F1</kbd> select and **Remote-Containers: Create Container Configuration File...** from the command palette.
   3. Select the Flutter definition.

3. To use latest-and-greatest copy of this definition from the repository:
   1. Clone this repository.
   2. Copy the contents of `containers/flutter/.devcontainer` to the root of your project folder.
   3. Start VS Code and open your project folder.

4. After following step 2 or 3, the contents of the `.devcontainer` folder in your project can be adapted to meet your needs.

5. Finally, press <kbd>F1</kbd> and run **Remote-Containers: Reopen Folder in Container** to start using the definition.

## Testing the definition

This definition includes some test code that will help you verify it is working as expected on your system. Follow these steps:

1. If this is your first time using a development container, please follow the [getting started steps](https://aka.ms/vscode-remote/containers/getting-started) to set up your machine.
2. Clone this repository.
3. Start VS Code, press <kbd>F1</kbd>, and select **Remote-Containers: Open Folder in Container...**
4. Select the `containers/flutter` folder.
5. After the folder has opened in the container, open the file `test/widget_test.dart` and click the **Run** Code Lens action above the sample test.
6. You should see the test appear in the Test view in the left sided bar and turn green.

**Note:** Right now it's only possible to run tests on the headless test device, it's not possible to run apps on real devices or emulators.

## License

Copyright (c) Microsoft Corporation. All rights reserved.

Licensed under the MIT License. See [LICENSE](https://github.com/Microsoft/vscode-dev-containers/blob/master/LICENSE).