# Codewind Language Server for Node.js Profiling

The Codewind language server for Node.js profiling annotates your Node.js code with code highlighting. By using profiling data gathered through Codewind load testing, the highlighting shows the relative time that is spent in JavaScript functions.

![Demonstration of Code Highlighting](res/img/quick-demo.gif)

## Running the extension with Visual Studio Code (VS Code)
1. Open a local project that you created with [Codewind](https://microclimate-dev2ops.github.io/installlocally) and profiled by using the [performance test](https://microclimate-dev2ops.github.io/performancetesting#performance-testing-your-project) feature.
2. Opening the project creates profiling data in a `load-test/[datestamp]/profiling.json` file in your Codewind project.
3. In VS Code, open a JavaScript file in your project. The extension highlights any lines that it finds in the profiling data and annotates them to show how often they were seen and where they were called from.
