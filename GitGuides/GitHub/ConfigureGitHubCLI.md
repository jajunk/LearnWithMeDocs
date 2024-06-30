# Guide to Install GitHub CLI and Configure to Work with GitHub on Linux

In this guide, we will walk you through the process of installing GitHub CLI (Command Line Interface) on Linux and configuring it to work with your GitHub account.

## Step 1: Install GitHub CLI

1. Open your terminal.
2. Run the following command to download the GitHub CLI package:

    ```
    sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-key C99B11DEB97541F0
    ```

3. Next, add the GitHub CLI repository to your system:

    ```
    sudo apt-add-repository https://cli.github.com/packages
    ```

4. Update your package list:

    ```
    sudo apt update
    ```

5. Finally, install GitHub CLI:

    ```
    sudo apt install gh
    ```

## Step 2: Authenticate with GitHub

1. To authenticate with GitHub, run the following command:

    ```
    gh auth login
    ```

2. Follow the prompts to authenticate with your GitHub account. You can choose to authenticate using your GitHub username and password, a personal access token, or by using your browser.

## Step 3: Configure GitHub CLI

1. Once authenticated, you can configure GitHub CLI by running the following command:

    ```
    gh config set editor <your-preferred-editor>
    ```

    Replace `<your-preferred-editor>` with the name of your preferred text editor (e.g., vim, nano, code).

2. You can also configure other settings such as the default repository visibility and the default branch name by running the following commands:

    ```
    gh config set prompt true
    gh config set git_protocol ssh
    ```

    Feel free to explore other configuration options by referring to the GitHub CLI documentation.

## Step 4: Test GitHub CLI

To test if GitHub CLI is working correctly, you can run the following command:

```
gh repo list
```

This command will list all the repositories associated with your GitHub account.

Congratulations! You have successfully installed GitHub CLI and configured it to work with GitHub on Linux.
