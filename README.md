# Codewind Node.js Profiler

Annotates your Node.js code with code highlighting for your hottest functions in your Codewind projects.

This extension provides code highlighting showing relative time spent in JavaScript functions based on profiling data gathered through Codewind Load Testing.

![Demonstration of Code Highlighting](res/img/quick-demo.gif)

## Usage

### Prerequisites

- The Codewind extension (available [here](https://marketplace.visualstudio.com/items?itemName=IBM.codewind)) installed in Visual Studio Code.
- A Node.js project bound to Codewind.

### With Visual Studio Code

- Open your Node.js project's Performance Dashboard by right-clicking on the project in the Codewind section of Visual Studio Code and selecting `Open Performance Dashboard`.
- Once the Performance Dashboard opens, click `Run Load Test`.
- This will create profiling data in a `load-test/[datestamp]/profiling.json` file in your Codewind project.
- In Visual Studio Code open a JavaScript file in your project.
- The extension will highlight any lines which were found in the profiling data and annotate them to show how often they were seen and where they were called from.
