🐍 **Python-to-Executable**

This repository provides a simple guide and tools to convert Python (.py) scripts into standalone executable (.exe) files. Convert your Python projects into easy-to-use executables to distribute to your clients or users without requiring them to install Python or any dependencies.

### Features:
- Convert Python scripts to standalone executable files.
- Easy-to-follow setup instructions.
- Compatible with Windows operating system.

### Requirements:
- Python 3.x installed on your system.
- [PyInstaller](https://www.pyinstaller.org/) library installed (`pip install pyinstaller`).

### Steps:
1. Save Python script with all the resources in one folder.
2. Open folder and press 'Shift + right click' select Open PowerShell window.
Run below commands:

- If no custom icon file were used.
```bash
pyinstaller myprogram.py
```
- With custom icon file (-F -i " " command).
```bash
pyinstaller -F -i "mylogo.ico" myprogram.py
```

- ( mylogo.ico = icon file name, myprogram.py = Python file name )
- If you want your executable application in one file `--onefile` and no console running `--noconsole` behind your application then go with the below line. If your app requires Windows Administrator permission then use `--uac-admin` command

```bash
pyinstaller -F -i "mylogo.ico" myprogram.py --onefile --noconsole
```
- If you want your executable application with additional file --add-data command, then go with the below line.
```bash
pyinstaller -F -i "mylogo.ico"--add-data "Additionalimage.png;." myprogram.py --onefile --noconsole
```
3. Go to dist folder and get application file, delete remain file except for resources.

   You successfully created your standalone application.

- However if you want your application (.exe) as setup file, windows installer will extract the installation resources from itself and manage their installation directly then, go with the below steps.

4. Install <a href="https://github.com/Abhijeetbyte/Python-Script-to-Application/blob/main/tools/innosetup-6.1.2.exe">Inno Setup</a> Compiler free application and Pyinstaller.

     Your computer must be running Python3 or newer.







### License:
This project is licensed under the [GNU License](LICENSE), which means you are free to use, modify, and distribute the code as per the terms and conditions specified in the license.

### Contributions:
Contributions to this project are welcome! If you find any issues or have suggestions for improvements, please feel free to open an issue or create a pull request.

### Support:
For any questions, feedback, or support, please contact us at mraheel.naseem@outlook.com
