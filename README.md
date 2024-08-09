# Guide: Setting up C with Visual Studio Code for Windows

### Table of Contents

- [Download and install Visual Studio Code](#download-and-install-visual-studio-code)
- [Setup MinGW for C/C++](#setup-mingw-for-cc)
- [Check MinGW Installation](#check-mingw-installation)
- [Set Up VS Code Extensions for C/C++](#set-up-vs-code-extensions-for-cc)
- [Test Your Final Setup](#test-your-final-setup)

## Download and install Visual Studio Code

1. Go to the [Visual Studio Code website](https://code.visualstudio.com/).
2. Click on the "Download" button for your operating system (Windows, macOS, or Linux).
3. Once the download is complete, run the installer.
4. Follow the on-screen instructions to complete the installation.

## Setup MinGW for C/C++

1. **Download the MinGW Zip Archive**

   - Visit the [Google Drive link for MinGW](YOUR_GOOGLE_DRIVE_LINK_HERE) and download the MinGW zip archive.

   #### ⚠️ **Important**: Save the MinGW zip file to `C:/` or else the script will not work correctly.

2. **Run the Setup Script**

   - Download the `setup_mingw.bat` script from [this direct download link](https://example.com/path/to/setup_mingw.bat).
   - Place the `setup_mingw.bat` script in the same directory as the downloaded MinGW zip file (`C:/`).
   - Double-click `setup_mingw.bat` to execute it. This script will extract the MinGW zip file, move the contents to `C:/mingw`, and add the `bin` directory to your system PATH.

## Check MinGW Installation

1. **Open Command Prompt**

   - Search for **Command Prompt** (`cmd`) in the Start menu and open it.

2. **Verify GCC Installation**

   - Type the following command and press `Enter` to check if MinGW is installed correctly:

     ```sh
     gcc --version
     ```

   - **Confirmation**: You should see output displaying the version of GCC (GNU Compiler Collection). For example:

     ```
     gcc (MinGW.org GCC-6.3.0-1) 6.3.0
     ```

   - If you see this output, it confirms that GCC is correctly installed and added to your system PATH.

3. **Troubleshooting**

   - If the commands are not recognized, ensure that:
     - You have saved and run the setup script properly.
     - You may need to restart Command Prompt or your computer for changes to take effect.

## Set Up VS Code Extensions for C/C++

These extensions will help you easily compile and run your C programs, as well as provide a range of tools and functionalities for C development.

1. **Install the C/C++ Compile Run Extension**

   - Open Visual Studio Code.
   - Go to the Extensions view by clicking the Extensions icon in the Activity Bar on the side of the window or by pressing `Ctrl+Shift+X`.
   - Search for **"C/C++ Compile Run"**. The search results should look like the screenshot below:
     ![C/C++ Compile Run Extension Search](https://imgur.com/GywMPBp.png)
   - Click on the **"C/C++ Compile Run"** extension by **danielpinto8zz6**, and then click **Install**. The installation process should be similar to the screenshot below:
     ![C/C++ Compile Run Extension Install](https://imgur.com/4YEfKRj.png)

   - Once the extension is installed, you may need to configure its settings. To do this, open the extension settings by navigating to:
     ![C/C++ Compile Run Extension Settings](https://imgur.com/fcveDqV.png)

   - In the extension's settings, find and check the option labeled:
     ![C/C++ Compile Run Extension Setting Option](https://imgur.com/EAlUO6J.png)

2. **Install the C/C++ Extension Pack**

   - In the Extensions view, search for **"C/C++ Extension Pack"**.
   - Click on the extension named **"C/C++ Extension Pack"** by **Microsoft**.
   ![C/C++ Extension Pack Search](https://imgur.com/lLqjcTh.png)
   - Click **Install**.
     ![C/C++ Extension Pack Install](https://imgur.com/pC2A7DN.png)

## Test Your Final Setup

1. **Create a New C File**

   - Open Visual Studio Code.
   - Go to **File** > **New File**.
   - Save the new file with a `.c` extension, for example: `hello.c`.

2. **Write a Simple C Program**

   - Enter the following code into your `hello.c` file:

     ```c
     #include <stdio.h>

     int main() {
         printf("Hello, World!\n");
         return 0;
     }
     ```

3. **Compile and Run the C Program**

   - To compile and run the program, press the `Run` button as shown below:
     ![Compile and Run Button](https://imgur.com/gimmiQX.png)

   - Alternatively, you can also press `F6` to compile and run.

   - You should see the output of your program in an external terminal prompt.
     ![Compile and Run Output](https://imgur.com/WJBvac2.png)

Following these steps ensures that your C development environment is set up correctly and allows you to start programming in C with Visual Studio Code.
