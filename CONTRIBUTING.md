# Contributing

We'd love for you to contribute to our source code and to make **Webex SDK Component Adapter** even better than it is today!
If you would like to contribute to this repository by adding features, enhancements or bug fixes, you must follow our process:

  1. [Create an issue](https://github.com/webex/sdk-component-adapter/issues) to propose your solution _before_ you get coding
  2. Let core members know about your proposal by posting a message in the [contributor's Webex Teams space](https://eurl.io/#Bk9WGfRcB)
  3. A core member will review your proposal and if necessary may suggest to have a meeting to better understand your approach
      - You are welcomed you join our [weekly review meeting](https://cisco.webex.com/m/f4ebbec6-c306-49ca-83f4-fb2d098fc946) (Thursdays, 11:30a-12:30p PST) to propose your contribution as well
  4. If your proposal is approved you should start coding at this point
  5. We recommend opening a draft PR to receive feedback before finalizing your solution
      - When opening a draft PR, specify with PR comments where in the code you would like to get feedback
  6. Before opening a PR ensure **all** [PR guidelines](#pull-request-guidelines) are followed
  7. Let core members know about your PR by posting a message in the [contributor's Webex Teams space](https://eurl.io/#Bk9WGfRcB)
  8. Core members will review the pull request and provide feedback when necessary
      - If a PR is too large, you may be asked to break it down into multiple smaller-scoped PRs
  9. Once the PR is approved by a core member, it will be merged
  10. Celebrate! Your code is released 🎈🎉🍻

## Opening an Issue

The title of a Bug or Enhancement should clearly indicate what is broken or desired. Use the description to explain possible solutions or add details and (especially for Enhancemnts) explain _how_ or _why_ the issue is broken or desired.

### Grammar

While quibbling about grammar in issue titles may seem a bit pedantic, adhering to some simple rules can make it much easier to understand a Bug or an Enhancement from the title alone. For example, is the title **"Browsers should support blinking text"** a bug or a feature request?

- Enhancements: The title should be an imperative statement of how things should be. **"Add support for blinking text"**

- Bugs: The title should be a declarative statement of how things are. **"Text does not blink"**

## Git Commit Guidelines

As part of the build process, commits are run through [conventional changelog](https://github.com/conventional-changelog/conventional-changelog) to generate the changelog. Please adhere to the following guidelines when formatting your commit messages.

### Commit Message Format

Each commit message consists of a **header**, a **body** and a **footer**. The header has a special format that includes a **type**, a **scope** and a **subject**:

```text
<type>(<scope>): <subject>
<BLANK LINE>
<body>
<BLANK LINE>
<footer>
```

The **header** is mandatory and the scope of the header is optional.

Any line of the commit message cannot be longer 100 characters! This allows the message to be easier to read on GitHub as well as in various git tools.

### Revert

If the commit reverts a previous commit, it should begin with `revert:`, followed by the header of the reverted commit. In the body it should say: `This reverts commit <hash>`., where the hash is the SHA of the commit being reverted.

### Type

Must be one of the following:

- **build**: Changes that affect the build system or external dependencies (example scopes: gulp, broccoli, npm)
- **ci**: Changes to our CI configuration files and scripts (example scopes: Circle, BrowserStack, SauceLabs)
- **docs**: Documentation only changes
- **feat**: A new feature
- **fix**: A bug fix
- **perf**: A code change that improves performance
- **refactor**: A code change that neither fixes a bug nor adds a feature
- **style**: Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc)
- **test**: Adding missing tests or correcting existing tests

### Scope

The scope should indicate what is being changed. Generally, these should match component or adapter names. For example, `WebexAdapter`, `PeopleAdapter`, `PeopleSDKAdapter` etc. Other than those, `tooling` tends to be the most common.

### Subject

The subject contains succinct description of the change:

- use the imperative, present tense: "change" not "changed" nor "changes"
- don't capitalize first letter
- no dot (.) at the end

### Body

Just as in the **subject** the imperative, present tense: "change" not "changed" nor "changes". The body should include the motivation for the change and contrast this with previous behavior.

### Footer

The footer should contain any information about **Breaking changes** and is also the place to reference GitHub issues that this commit **closes**.

**Breaking Changes** should start with the word `BREAKING CHANGE:` with a space or two newlines. The rest of the commit message is then used for this.

### Static Analysis (e.g. linting)

We use eslint as a part of our static analysis step. Before contributing any code, please be sure to install eslint and be sure to following the instructions to correctly install peerDependnencies <https://www.npmjs.com/package/@webex/eslint-config-react>

## Pull Request Guidelines

Pull requests must include code documentation, tests, follow code style and commits format.
