# Getting Started Guide

This guide will help you get started using **welcome bot** on your own repositories. For more information on what this bot does, check out the [README](../README.md).

## Installing the bot

The bot works by providing a message on a contributor's first issue, pull request, or merged pull request. In order to scan a repository, the app must be installed on that repository. To install the app, use the following instructions:

1. [Install the bot](https://github.com/apps/welcome) on the intended repositories. The plugin requires the following Permissions and Events:

- Pull requests: Read & Write
- Issues: Read & Write

## Creating the config

The bot is designed to create messages when a user creates an issue, open a pull request, or merges a pull request. These messages are based on a config file in your repository. You will need to create a config file with the messages you want **welcome** to use. Your `.github/config.yml` should look something like this:

```
# Configuration for welcome - https://github.com/behaviorbot/welcome

# Configuration for new-issue-welcome - https://github.com/behaviorbot/new-issue-welcome

# Comment to be posted to on PRs from first time contributors in your repository
newPRWelcomeComment: >
  Thanks for opening this pull request! Please check out our contributing guidelines.

# Configuration for first-pr-merge - https://github.com/behaviorbot/first-pr-merge

# Comment to be posted to on pull requests merged by a first time user
firstPRMergeComment: >
  Congrats on merging your first pull request! We here at behaviorbot are proud of you!

# It is recommended to include as many gifs and emojis as possible!
```

### Example Messages

# Configuration for new-issue-welcome - https://github.com/behaviorbot/new-issue-welcome

# Comment to be posted to on first time issues
newIssueWelcomeComment: |
  👋 Thanks for opening your first issue here! If you're reporting a 🐞 bug, please make sure you include steps to reproduce it. We get a lot of issues on this repo, so please be patient and we will get back to you as soon as we can.

  To help make it easier for us to investigate your issue, please follow the [contributing guidelines](https://github.com/electron/electron/blob/master/CONTRIBUTING.md).

# Configuration for new-pr-welcome - https://github.com/behaviorbot/new-pr-welcome

# Comment to be posted to on PRs from first time contributors in your repository
newPRWelcomeComment: |
  💖 Thanks for opening this pull request! 💖

  We use [semantic commit messages](https://github.com/electron/electron/blob/master/docs/development/pull-requests.md#commit-message-guidelines) to streamline the release process. Before your pull request can be merged, you should **update your pull request title** to start with a semantic prefix.

  Examples of commit messages with semantic prefixes:

  - `fix: don't overwrite prevent_default if default wasn't prevented`
  - `feat: add app.isPackaged() method`
  - `docs: app.isDefaultProtocolClient is now available on Linux`

  Things that will help get your PR across the finish line:

  - Follow the JavaScript, C++, and Python [coding style](https://github.com/electron/electron/blob/master/docs/development/coding-style.md).
  - Run `npm run lint` locally to catch formatting errors earlier.
  - Document any user-facing changes you've made following the [documentation styleguide](https://github.com/electron/electron/blob/master/docs/styleguide.md).
  - Include tests when adding/changing behavior.
  - Include screenshots and animated GIFs whenever possible.

  We get a lot of pull requests on this repo, so please be patient and we will get back to you as soon as we can.

# Configuration for first-pr-merge - https://github.com/behaviorbot/first-pr-merge

# Comment to be posted to on pull requests merged by a first time user
firstPRMergeComment: >
  Congrats on merging your first pull request! 🎉🎉🎉

# Configuration for trop - https://github.com/codebytere/trop

watchedProject:
  name: Backports

authorizedUsers:
  - zhongweili
  - alexeykuzmin
  - ckerr
  - codebytere
  - deepak1556
  - jkleinsc
  - MarshallOfSound
  - nitsakh
  - nornagon
  - zcbenz

