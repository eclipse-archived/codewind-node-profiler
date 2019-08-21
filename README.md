# Codewind Language Server for Node.js Profiling

The Codewind language server for Node.js profiling annotates your Node.js code with code highlighting. By using profiling data gathered through Codewind load testing, the highlighting shows the relative time that is spent in JavaScript functions.

![Demonstration of Code Highlighting](res/img/quick-demo.gif)

## Running the extension with Visual Studio Code (VS Code)
1. Open a local project that you created with [Codewind](https://microclimate-dev2ops.github.io/installlocally) and profiled by using the [performance test](https://microclimate-dev2ops.github.io/performancetesting#performance-testing-your-project) feature.
2. Opening the project creates profiling data in a `load-test/[datestamp]/profiling.json` file in your Codewind project.
3. In VS Code, open a JavaScript file in your project. The extension highlights any lines that it finds in the profiling data and annotates them to show how often they were seen and where they were called from.

## Running the Extension

With Visual Studio Code:

- Clone this repository locally.
- Run `npm install` in the cloned `codewind-ls-node-prof` folder. This installs all necessary npm modules in both the client and server folder
- Open the clone of this repository in Visual Studio Code.
- Press Ctrl+Shift+B (Cmd+Shift+B on Mac) to compile the client and server.
- Switch to the Debug viewlet.
- Select `Launch Client` from the drop down and press the Run icon.
- If you want to debug the server as well use the launch configuration `Attach to Server`.

## Testing

Setup:

- Run `npm install` in the `codewind-ls-node-prof` folder.

In Visual Studio Code:

- Press Ctrl+Shift+B (Cmd+Shift+B on Mac) to compile the client and server.
- Run `npm run prepare-tests` in the `vscode/client` folder.
- Switch to the Debug viewlet.
- Select `Language Server E2E Test` from the drop down.
- Run the test config.
- An additional editor will momentarily open while the tests are run. It will close automatically once they are complete.
- Switch to the output view with Ctrl+Shift+U (Cmd+Shift+U on Mac) to see the results of the tests.

## Building/Installing the Extension

To build a `.vsix` extension package that can then be installed/published:

- Run `npm install` in the `codewind-ls-node-prof` folder.
- Install the `vsce` package globally with `npm install -g vsce`.
- Run `vsce package` in the `codewind-ls-node-prof` folder.
- A `.vsix` file will then be generated.

To install the extension:

- Run `code --install-extension <name of generated vsix file>` in the `codewind-ls-node-prof` folder.
- Restart Visual Studio Code.
- The extension should appear in your list of installed extensions.

For more information refer to: <https://code.visualstudio.com/api/working-with-extensions/publishing-extension>