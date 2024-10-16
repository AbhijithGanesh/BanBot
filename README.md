# 🚨 GitHub Moderation Bot - NSFW Content Filter & Zombie User Blocker

Welcome to the **GitHub Moderation Bot**! This bot automatically moderates issues and discussions on your repository by preventing ghost or zombie users (accounts with little or no activity) from creating issues containing NSFW (Not Safe For Work) content.

## 📋 Features

- **Block NSFW Content**: Automatically scans and flags issues or discussions containing inappropriate or NSFW content.
- **Zombie User Detection**: Identifies and restricts ghost or zombie users (inactive or new accounts with low engagement) from creating potentially spam issues.
- **Customizable Filters**: Ability to customize the filter keywords and criteria for ghost user detection.
- **Automated Response**: Sends a warning message or automatically moderates the issues if the bot detects violations.
- **Manual Overrides**: Admins can manually override bot actions or whitelist users.

## 🚀 Getting Started

### Prerequisites

To use this bot, you'll need:

- A GitHub repository
- Basic understanding of GitHub Actions
- A GitHub API Token with repo permissions

### Usage

Once the bot is installed and the workflow is active, it will automatically monitor issues and discussions created in your repository. If a flagged term is detected, or if the user has low activity, the bot will:

- Moderate the issue
- Leave a warning message as a comment

Admins can manually reopen closed issues or whitelist specific users.

## 🛠 Customization

- **NSFW Keywords**: Add or remove keywords from the `NSFW_KEYWORDS` array in the YAML file to suit your project's needs.
- **Zombie User Threshold**: Adjust `MIN_ACTIVITY` to modify the threshold for blocking ghost users.
- **Actions**: Change how the bot handles violations, such as leaving a comment instead of closing the issue.

## 📄 License

This project is licensed under the GPL License - see the [LICENSE](LICENSE) file for details.

## Made using

[OctoKit](https://github.com/khornberg/octokit.py)
