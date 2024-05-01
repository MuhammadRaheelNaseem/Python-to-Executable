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

![image](https://github.com/MuhammadRaheelNaseem/Python-to-Executable/assets/63813881/0264cbe5-d664-4fb5-a2b4-07c803a18cf1)

![image](https://github.com/MuhammadRaheelNaseem/Python-to-Executable/assets/63813881/fdcece78-3688-4c26-a852-6565f22c5ad7)

![image](https://github.com/MuhammadRaheelNaseem/Python-to-Executable/assets/63813881/84a89cca-29b4-4ebe-be3b-b47218360220)

![image](https://github.com/MuhammadRaheelNaseem/Python-to-Executable/assets/63813881/c82b306b-caa2-45fc-9a21-7e953aff4c39)

![image](https://github.com/MuhammadRaheelNaseem/Python-to-Executable/assets/63813881/d29654d7-2163-44d5-af12-0663b4196150)



3. Go to dist folder and get application file, delete remain file except for resources.

   You successfully created your standalone application.

- However if you want your application (.exe) as setup file, windows installer will extract the installation resources from itself and manage their installation directly then, go with the below steps.

4. Install <a href="https://github.com/Abhijeetbyte/Python-Script-to-Application/blob/main/tools/innosetup-6.1.2.exe">Inno Setup</a> Compiler free application and Pyinstaller.

     Your computer must be running Python3 or newer.


![image](https://github.com/MuhammadRaheelNaseem/Python-to-Executable/assets/63813881/7bc1aedd-72cb-40ea-893f-8e420c90e040)


![image](https://github.com/MuhammadRaheelNaseem/Python-to-Executable/assets/63813881/e296375f-bbf1-4396-84e5-6ba2c9afcf13)


![image](https://github.com/MuhammadRaheelNaseem/Python-to-Executable/assets/63813881/526f4380-a4c5-4a7a-853b-a2fd0c0ffacd)


![image](https://github.com/MuhammadRaheelNaseem/Python-to-Executable/assets/63813881/72760560-c2dc-4d94-b525-f0dac9c0c982)


![image](https://github.com/MuhammadRaheelNaseem/Python-to-Executable/assets/63813881/fb668d2e-52cb-4e44-b732-50158706801a)


![image](https://github.com/MuhammadRaheelNaseem/Python-to-Executable/assets/63813881/115198f5-0f03-47b1-8c3c-781d08e191e6)


![image](https://github.com/MuhammadRaheelNaseem/Python-to-Executable/assets/63813881/3f34868a-ef43-41f2-9227-b6ddecb87ef0)

![image](https://github.com/MuhammadRaheelNaseem/Python-to-Executable/assets/63813881/f97dd48c-4c4c-437e-a3c8-7a7bd4d831f1)

![image](https://github.com/MuhammadRaheelNaseem/Python-to-Executable/assets/63813881/8eebc943-3d1a-48e9-9fe5-e22da76b93fc)

![image](https://github.com/MuhammadRaheelNaseem/Python-to-Executable/assets/63813881/d0303e9d-84f8-4907-ab36-0c9251611e60)

![image](https://github.com/MuhammadRaheelNaseem/Python-to-Executable/assets/63813881/a2902d69-e8c4-4fd1-b136-2504fe70b76f)








### License:
This project is licensed under the [GNU License](LICENSE), which means you are free to use, modify, and distribute the code as per the terms and conditions specified in the license.

### Contributions:
Contributions to this project are welcome! If you find any issues or have suggestions for improvements, please feel free to open an issue or create a pull request.

### Support:
For any questions, feedback, or support, please contact us at mraheel.naseem@outlook.com
