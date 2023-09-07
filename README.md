
# Standards Converter

This is a guide for how to convert level runs in `.DAT` format to an excel file. Please reach out to me at BMoyle@jmt.com or on Teams if you have any questions.

# Installation
Installation has been streamlined to a `.BAT` file. In the event that the batch file fails to install the requirements, below will also be the steps for manual installation.

### Simple install
![Image of Install.bat](https://github.com/JMT-bmoyle/LevelsToXlsx/blob/main/Images/Install.png?raw=true)

In the directory `Q:\AZURE_HVMD\00-Reality_Capture\Sandbox\bmoyle\LevelsToXlsx` double click on `Install.bat`. This will install [Python3.10](https://www.python.org/downloads/release/python-3107/), Upgrade [PIP](https://pypi.org/project/pip/), and install the required modules [openpyxl](https://pypi.org/project/openpyxl/) and [tqdm](https://pypi.org/project/tqdm/).

### Manual install
In the directory `Q:\AZURE_HVMD\00-Reality_Capture\Sandbox\bmoyle\LevelsToXlsx`: 
- open `python-3.10.7-amd64.exe`
- Uncheck "Install launcher for all users (recommended)" and check "Add Python 3.10 to PATH"
- Click Install Now
- In commandline, run the following:
    - `python.exe -m pip install --upgrade pip`
    - `pip install openpyxl`
    - `pip install tqdm`
- Type `py` in commandline to ensure python is installed
- In the python terminal run `import openpyxl; import tqdm` to ensure the modules are installed.

# Usage
![Image of LevelsToXlsx.py](https://github.com/JMT-bmoyle/LevelsToXlsx/blob/main/Images/Script.png?raw=true)

Double click on `LevelsToXlsx.py`. A window will pop up, then an explorer dialog will appear.

![Image of selecting DAT file](https://github.com/JMT-bmoyle/LevelsToXlsx/blob/main/Images/FindDAT.png?raw=true)

As seen in the bottom right corner, it is asking for our `.DAT` file. Navigate to it and select it.

![Image of finished writing](https://github.com/JMT-bmoyle/LevelsToXlsx/blob/main/Images/Finished.png?raw=true)

The conversion process is finished! A pop up should tell you that it has completed. Click `OK`, and a Excel file will be in the same location as the original `.DAT`. This is the file you want to use.

# Errors and Cleanup

If the program closes without finishing, please check the `.DAT` to ensure that there is a Start-Line and an End-Line. If the level run was not finished properly this could cause it to fail. Also make sure that the file is following the normal formatting, as changing the way the file is structured will break the script.

### If issues continue, please reach out!
