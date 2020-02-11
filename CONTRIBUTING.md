
# Contributing

## Running the Extension

With Visual Studio Code:

- Clone this repository locally.
- Run `npm install` in the cloned `codewind-node-profiler` folder. This installs all necessary npm modules in both the client and server folder
- Open the clone of this repository in Visual Studio Code.
- Press Ctrl+Shift+B (Cmd+Shift+B on Mac) to compile the client and server.
- Switch to the Debug viewlet.
- Select `Launch Client` from the drop down and press the Run icon.
- If you want to debug the server as well use the launch configuration `Attach to Server`.

## Testing

Setup:

- Run `npm install` in the `codewind-node-profiler` folder.

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

- Run `npm install` in the `codewind-node-profiler` folder.
- Install the `vsce` package globally with `npm install -g vsce`.
- Run `vsce package` in the `codewind-node-profiler` folder.
- A `.vsix` file will then be generated.

To install the extension:

- Run `code --install-extension <name of generated vsix file>` in the `codewind-node-profiler` folder.
- Restart Visual Studio Code.
- The extension should appear in your list of installed extensions.

For more information refer to: <https://code.visualstudio.com/api/working-with-extensions/publishing-extension>
=======
## Contributing
Thank you for your interest in contributing to Codewind. We welcome your additions to this project.

#### Signing the Eclipse Contributor Agreement (ECA)
Before you can contribute to any Eclipse project, you need to sign the [Eclipse Contributor Agreement (ECA)](https://www.eclipse.org/legal/ECA.php).
1. To verify that you signed the ECA, sign in to [https://accounts.eclipse.org/ your Eclipse account].
2. View your **Status** and make sure that a check mark appears with the **Eclipse Contributor Agreement**.
3. If the check mark does not appear, click the **Eclipse Contributor Agreement** in the **Status** box to go to the agreement that you need to sign.
4. Fill the form and click the **Accept** button.

#### Associating your Eclipse profile with your GitHub ID
1. From your Eclipse account, select **Edit Profile**.
2. On the **Personal Information** tab, go to the **Social Media Links** section and add your GitHub user name to the **GitHub Username** field.
3. Answer the **Have you changed employers** question.
4. Enter your Eclipse password in the **Current password** field and then click **Save**.

For more information about Codewind workflows, see the [Codewind GitHub Workflows wiki](https://wiki.eclipse.org/Codewind_GitHub_Workflows).

#### Checking if your issue is already addressed
- Search the [list of issues](https://github.com/eclipse/codewind/issues) to see if your issue has already been raised.
- See the [Codewind documentation](https://www.eclipse.org/codewind/docindex.html) to see if existing documentation addresses your question or concern.

#### Creating a new issue
If you do not see your issue, please [select the issue type in the Codewind repository to open a new issue](https://github.com/eclipse/codewind/issues/new/choose).
- **Bugs:** Complete the bug template to report problems found in Codewind.
- **Enhancements:** Complete the enhancement template to suggest improvements to Codewind.
- **Questions:** Complete the question template to ask a question about Codewind.

## Contact us
If you have questions, please visit us on [Mattermost](https://mattermost.eclipse.org/eclipse/channels/eclipse-codewind).

