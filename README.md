# Selenium Script for Green City Practical Task

This project contains a script created with **Selenium IDE v3.17.2** and is tested to work stably with the following versions:

- **selenium-side-runner**: v3.14.0
- **Node.js**: v18.20.4 (LTS) or v22.11.0 (LTS)

## Script Information

- **Author**: Maxim
- **Script Version**: v1.0.0

## Prerequisites

Make sure you have Node.js and npm installed on your system. Follow these steps to install the required versions if needed.

### Installing Node.js

1. Go to the official Node.js website: [https://nodejs.org/en/download/prebuilt-installer](https://nodejs.org/en/download/prebuilt-installer).
2. Download and install the latest LTS version (v18.20.4 or v22.11.0 is recommended for compatibility).
3. After installation, open the Command Prompt to verify the installation:
   - Press **Win + R**, type `cmd`, and hit **Enter**.
   - Run the following command to check the Node.js version:

     ```cmd
     node -v
     ```

     You should see a version number (e.g., `v18.20.4`).

4. Confirm `npm` is installed by checking its version with:

    ```cmd
    npm -v
    ```

    If `npm` is installed, a version number will appear.

### Installing Selenium Side Runner and ChromeDriver

1. **Install Selenium Side Runner** (required version: 3.14.0):

    ```cmd
    npm install -g selenium-side-runner@3.14.0
    ```

2. **Install ChromeDriver**:

    ```cmd
    npm install -g chromedriver
    ```

3. **Verify installed versions** to ensure everything is set up correctly:

    ```cmd
    selenium-side-runner --version
    chromedriver --version
    ```

    You should see `selenium-side-runner` version `3.14.0` and a version number for `chromedriver` (e.g., `114.0.5735.90` — the version may vary).

## Running the Script

1. Open the Command Prompt **cmd** (Win + R → type `cmd` → Enter).
2. Navigate to the folder containing your `.side` file. Use the `cd` command, for example:

    ```cmd
    cd C:\path\to\your\side\file
    ```

3. Run the script using the following command:

    ```cmd
    selenium-side-runner 05_Practical_TaskgreenCity_hw.side
    ```
 This will execute the script specified in the `.side` file, see the [video instructions](https://youtu.be/x7uLkua6r8c).

## Script Information

- :warning: Case you encounter an error:
   `The ChromeDriver could not be found on the current PATH. Please download the latest version of the ChromeDriver from http://chromedriver.storage.googleapis.com/index.html and ensure it can be found on your PATH.`

:white_check_mark: **The steps below may assist you:**
    1. Open the folder of node package manager(npm), better to search it using search by path to selenium-side-runner, use the command below
    2. Find the chromedriver.exe file.
    3. Move it up to the root folder of npm.
  
    where selenium-side-runner
    
 Watch the video with the [error solution](https://youtu.be/VCUVo2pNqNg).
  

- :warning: If the Green City website loads in Ukrainian, it is due to the localization of our device and the script below may help resolve the issue. It also runs the script without GIU

:white_check_mark: **Run this code to include a `.side.yaml` file with instructions to make it run silently (without GIU):**

    selenium-side-runner 05_Practical_TaskgreenCity_hw.side --config .side.yaml


