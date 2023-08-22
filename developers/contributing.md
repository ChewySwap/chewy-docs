# 👍 Contributing

## Contributing

Thank you for expressing your interest in contributing to ChewySwap!

ChewySwap is an open-source project. If you want to contribute to the project, this section is here to guide you through your first steps with the ChewySwap team. Before starting any development, we highly encourage you to submit an issue on Github in order to discuss the problem, and the solution with the team.

### Setup your dev environment <a href="#setup-your-dev-environment" id="setup-your-dev-environment"></a>

Install [yarn](https://classic.yarnpkg.com/lang/en/docs/install/) If you haven't.

1. 1.Fork and clone the [repository](https://github.com/pancakeswap/pancake-frontend)​\
   `git clone [fork_repo_url]`
2. 2.Add [upstream](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/configuring-a-remote-for-a-fork) remote. E.g.\
   `git remote add upstream git@github.com:pancakeswap/pancake-frontend.git`
3. 3.Make sure you have the latest version of the default branch ( `develop` )\
   `git checkout develop$ git pull upstream develop`
4. 4.Create your own branch and install dependencies\
   `git checkout -b branch-name`\
   `yarn`
5. 5.Happy coding 🎉

### Coding rules <a href="#coding-rules" id="coding-rules"></a>

We try to maintain as much consistency as we can between each of our repository. Your pull request has more chances to be accepted if you follow the following rules, and write high quality code. **Let's get started** 💪

### Use the UIKit <a href="#use-the-uikit" id="use-the-uikit"></a>

{% hint style="warning" %}
Check the [UI Kit](https://github.com/pancakeswap/pancake-frontend/tree/master/packages/uikit) before you start doing anything. A lot of components are already created, and we don't want that you waste your time reinventing the wheel 😉
{% endhint %}

If a variant of a component needs to be created, use the corresponding component in the UI Kit as a base. For example:

```jsx
import styled from 'styled-components'
import { Button } from '@pancakeswap/uikit'
​
const NewButtonVariant = styled(Button)`// custom styles here`
```

### Use the tools! <a href="#use-the-tools" id="use-the-tools"></a>

Most of our repos use [Typescript](https://www.typescriptlang.org/docs), [ESLint](https://eslint.org/docs/user-guide/getting-started), and [Prettier](https://prettier.io/). Make sure you're familiar with Typescript’s best practices and enable an ESLint and Prettier plugin for your IDE.Make sure your code is formatted with Prettier and is free from any ESLint error before you submit a pull request.

#### Some good practices <a href="#some-good-practices" id="some-good-practices"></a>

* Keep components as small and ["dumb"](https://en.wikipedia.org/wiki/Pure\_function) as possible.
* Use [Composition over Inheritance](https://reactjs.org/docs/composition-vs-inheritance.html).
* Keep in mind that your code will be read and maintained by several other developers. Make it as clear and easy to update as possible._​_

### Creating your pull request <a href="#creating-your-pull-request" id="creating-your-pull-request"></a>

Your code is ready to be submitted for review, congratulations🥳

* All pull requests **must** have a description of what the PR is trying to accomplish.
* Keep pull requests **as small as possible**. Larger pull requests should be broken up into smaller chunks with a dedicated base branch. Please tag the PR's that are merging into your base branch with the `epic` tag.
* If possible self-review your PR and **add comments** where additional clarification is needed.

Create a [draft PR](https://github.blog/2019-02-14-introducing-draft-pull-requests/) as soon as possible so we can view your ongoing progress.

#### Pull Request Title <a href="#pull-request-title" id="pull-request-title"></a>

Our Pull Request Title follow [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/) using [commitlint](https://commitlint.js.org/#/).‌ _More at_ [_Angular's guidelines_](https://github.com/angular/angular/blob/22b96b9/CONTRIBUTING.md#type)_​_

| Type         | Description                                                                                                 |
| ------------ | ----------------------------------------------------------------------------------------------------------- |
| **build**    | Changes that affect the build system or external dependencies (example scopes: gulp, broccoli, npm)         |
| **ci**       | Changes to our CI configuration files and scripts (example scopes: Travis, Circle, BrowserStack, SauceLabs) |
| **docs**     | Documentation only changes                                                                                  |
| **feat**     | A new feature                                                                                               |
| **fix**      | A bug fix                                                                                                   |
| **perf**     | A code change that improves performance                                                                     |
| **refactor** | A code change that neither fixes a bug nor adds a feature                                                   |
| **style**    | Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc)      |
| **test**     | Adding missing tests or correcting existing tests                                                           |

**Thanks for helping us making ChewySwap even more awesome** ❤
