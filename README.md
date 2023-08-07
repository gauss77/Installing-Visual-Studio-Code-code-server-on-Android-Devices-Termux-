# Installing Visual Studio Code (code-server) on Android Devices (Termux)

This guide will walk you through the steps to install Visual Studio Code (code-server) on your Android device using Termux.

## Prerequisites

1. Install Termux from the GitHub repository or [termux.com](https://termux.com).

## Instructions

1. Update system packages in Termux:
   ```
   pkg update -y
   ```

2. Add the Tur repository:
   ```
   pkg install tur-repo
   ```

3. Install code-server:
   ```
   pkg install code-server
   ```

4. Check the installed version of code-server:
   ```
   code-server --version
   ```

5. Try running code-server with no authentication:
   ```
   code-server --auth none
   ```

6. Open your browser and navigate to `127.0.0.1:8080` to access the code-server interface.

## Bonus

If you want to run code-server on a PC browser, you can forward the port using adb:
```
adb forward tcp:8080 tcp:8080
```
Then, open your PC's browser and access `localhost:8080` to use code-server remotely.

Enjoy coding on your Android device using Visual Studio Code! If you encounter any issues during the installation process, feel free to seek help from the Termux community or refer to the official documentation. Happy coding!