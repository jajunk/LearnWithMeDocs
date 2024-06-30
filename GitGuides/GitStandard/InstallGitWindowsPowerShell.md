# Install Git on Windows from Command Line (PowerShell)

To install Git on Windows using the command line (PowerShell), follow these steps:

1. Open PowerShell: Press `Win + X` and select "Windows PowerShell" from the menu.

2. Check if Git is already installed: Run the following command to check if Git is already installed on your system:
    ```
    git --version
    ```

    If Git is already installed, you will see the version number. If not, proceed to the next step.

3. Download Git: Run the following command to download the Git installer:
    ```
    Invoke-WebRequest -Uri "https://git-scm.com/download/win" -OutFile "git-installer.exe"
    ```

4. Install Git: Run the following command to start the Git installation:
    ```
    Start-Process -Wait -FilePath "git-installer.exe"
    ```

    Follow the prompts in the installer to complete the installation.

5. Verify the installation: Run the following command to verify that Git has been installed successfully:
    ```
    git --version
    ```

    You should see the version number of Git displayed.

That's it! You have successfully installed Git on Windows using the command line (PowerShell).
