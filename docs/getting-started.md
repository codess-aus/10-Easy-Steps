Placeholder

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

Welcome to our repository! Thanks for adding an issue, if you are reporting a bug or a feature request, please make sure to assign a label to this issue.
