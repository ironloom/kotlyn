**Note:** If you plan on making a big and serious project, Kotlyn is not the library you are looking for. For big projects you probably want to use [gradle](https://gradle.org/install/#manually). While the `kotlinc` (the library which Kotlyn is based on) is pretty powerful, it's nowhere near as useful as gradle. 


---

```    
  _   __      _   _             
 | | / /     | | | |              💙💙💜💛💛💛
 | |/ /  ___ | |_| |_   _ _ __    🩵💙💛💛💛  
 |    \ / _ \| __| | | | | '_ \   🩷🧡💛💛    
 | |\  \ |_| | |_| | |_| | | | |  🩷🧡🧡💜    
 \_| \_/\___/ \__|_|\__, |_| |_|  🧡🧡🩵💙💜  
                     __/ |        🧡🩵🩵💙💙💜
                    |___/
```
# Kotlyn
> **CURRENTLY WINDOWS ONLY!**<br>
> If everything goes as planned the unix based version will be out by May 2024.<br>

Kotlyn is a toolkit to build and run Kotlin appications from the command line. This "python package" hijacks the pypi package manager/distributor to install Kotlin's latest version on your system. Apart from installing JetBrain's `kotlinc` terminal tool, Kotlyn provides a ✨ **new and shiny CLI** ✨ to run and build kotlin files.


## Installation Guide
It's really easy, don't worry! 

1. **Make sure python 🐍 is installed**
```powershell
python --version
```

2. **Use pip to install the CLI**
```powershell
python -m pip install --upgrade kotlyn
```

3. **Run the setup**
```powershell
python -m kotlyn !setup
```

4. **Check if the installation is correct ✅**<br>
Once the setup is installed, you can just use the `kotlyn` keyword to access the CLI.
```powershell
kotlyn !version
```

## Usage
> **CURRENTLY ALL `.KT` FILES IN THE ENTRY FILE'S DIR ARE LINKED & COMPILED** <br>
*A fix/feature is on the way*

After runing the setup command, you are able to use the shorthand `kotlyn` instead of `python -m kotlyn`.

### Run a kotlin (`.kt`) file
This will build the `.jar` file in kotlyn's temp folder and will automatically delete it after the program has finished.

To run ▶️ the `Main.kt`  just do
```powershell
kotlyn Main.kt
```

### Build the `Main.jar` file
This will build the `Main.jar` file in the same directory where your entry kotlin file is located.

To build 🛠️ the `Main.kt` into `Main.jar` just do
```powershell
kotlyn --build Main.kt
```