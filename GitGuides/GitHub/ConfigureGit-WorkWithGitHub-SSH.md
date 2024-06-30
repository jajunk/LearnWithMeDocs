# Configure Git to Work with GitHub via Terminal and SSH on Linux

In this guide, we will walk you through the steps to configure Git to work with GitHub via terminal and SSH on Linux.

## Prerequisites
Before you begin, make sure you have the following:

1. A GitHub account. If you don't have one, you can create it at [github.com](https://github.com).
2. Git installed on your Linux machine. If Git is not installed, you can install it by running the following command in your terminal:
    ```
    sudo apt-get install git
    ```

## Step 1: Generate SSH Key
To work with GitHub via SSH, you need to generate an SSH key. Follow these steps:

1. Open your terminal.
2. Run the following command to generate a new SSH key:
    ```
    ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
    ```
    Replace `your_email@example.com` with the email associated with your GitHub account.
3. Press Enter to accept the default file location and passphrase (or set your own).
4. The SSH key will be generated and saved in the default location (`~/.ssh/id_rsa`).

## Step 2: Add SSH Key to GitHub
Now that you have generated an SSH key, you need to add it to your GitHub account. Follow these steps:

1. Copy the SSH key to your clipboard by running the following command:
    ```
    cat ~/.ssh/id_rsa.pub | xclip -selection clipboard
    ```
    If you don't have `xclip` installed, you can install it by running `sudo apt-get install xclip`.
2. Go to [github.com](https://github.com) and log in to your GitHub account.
3. Click on your profile picture in the top-right corner and select **Settings**.
4. In the left sidebar, click on **SSH and GPG keys**.
5. Click on **New SSH key**.
6. Give your SSH key a title (e.g., "Linux SSH Key") and paste the key into the **Key** field.
7. Click on **Add SSH key**.

## Step 3: Test SSH Connection
To test if your SSH connection is working correctly, follow these steps:

1. Open your terminal.
2. Run the following command:
    ```
    ssh -T git@github.com
    ```
3. You should see a message like `Hi username! You've successfully authenticated...`.

## Step 4: Configure Git with GitHub
To configure Git to work with GitHub, follow these steps:

1. Open your terminal.
2. Set your Git username by running the following command:
    ```
    git config --global user.name "Your Name"
    ```
    Replace "Your Name" with your GitHub username.
3. Set your Git email by running the following command:
    ```
    git config --global user.email "your_email@example.com"
    ```
    Replace `your_email@example.com` with the email associated with your GitHub account.
4. Run the following command to enable credential caching:
    ```
    git config --global credential.helper cache
    ```

## Conclusion
Congratulations! You have successfully configured Git to work with GitHub via terminal and SSH on Linux. You can now start using Git to collaborate with others on GitHub.
