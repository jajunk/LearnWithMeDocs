# Guide to Create and Install GitHub Personal Access Tokens on Linux

GitHub Personal Access Tokens are used to authenticate and authorize access to your GitHub account. They can be used for various purposes, such as accessing the GitHub API, interacting with repositories, and performing actions on behalf of your account.

Here's a step-by-step guide to creating and installing GitHub Personal Access Tokens on Linux:

1. Open your web browser and go to the GitHub website (https://github.com).

2. Log in to your GitHub account.

3. Click on your profile picture in the top-right corner of the page and select "Settings" from the dropdown menu.

4. In the left sidebar, click on "Developer settings".

5. In the left sidebar, click on "Personal access tokens".

6. Click on the "Generate new token" button.

7. Give your token a descriptive name in the "Note" field. This will help you identify its purpose later.

8. Select the scopes or permissions you want to grant to the token. Be cautious and only select the necessary permissions to ensure the security of your account.

9. Click on the "Generate token" button at the bottom of the page.

10. GitHub will generate a new personal access token for you. Make sure to copy it immediately as it will not be shown again.

11. Open a terminal on your Linux machine.

12. Run the following command to create a new environment variable for your token:

    ```bash
    export GITHUB_TOKEN=YOUR_TOKEN_HERE
    ```

    Replace `YOUR_TOKEN_HERE` with the actual token you copied in the previous step.

13. To make the token available in all terminal sessions, add the above command to your shell's configuration file (e.g., `~/.bashrc` or `~/.zshrc`).

14. Save the changes to the configuration file and restart your terminal or run the following command to reload the configuration:

    ```bash
    source ~/.bashrc
    ```

15. You can now use the `GITHUB_TOKEN` environment variable in your scripts or command-line tools to authenticate with GitHub.

Remember to keep your personal access tokens secure and avoid sharing them with others. If you suspect that your token has been compromised, you can revoke it and generate a new one following the same steps.
