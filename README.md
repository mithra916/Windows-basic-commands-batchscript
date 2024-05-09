# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript
# AIM:
To execute Windows basic commands and batch scripting
# DESIGN STEPS:
### Step 1:
Navigate to any Windows environment installed on the system or installed inside a virtual environment like virtual box/vmware 
### Step 2:
Write the Windows commands / batch file
Save each script in a file with a .bat extension.
Ensure you have the necessary permissions to perform the operations.
Adapt paths as needed based on your system configuration.
### Step 3:
Execute the necessary commands/batch file for the desired output. 
# WINDOWS COMMANDS:
## Exercise 1: Basic Directory and File Operations
Create a directory named "MyLab" on the desktop.
## COMMAND AND OUTPUT
mkdir %userprofile%\Desktop\MyLab 

![image](https://github.com/mithra916/Windows-basic-commands-batchscript/assets/149986612/9f99712a-257d-4722-a577-cb087c7d2c83)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.
## COMMAND AND OUTPUT
cd %userprofile%\Desktop\MyLab

![image](https://github.com/mithra916/Windows-basic-commands-batchscript/assets/149986612/8ca1d2c0-c60e-4edf-b256-787f84007bce)

![image](https://github.com/mithra916/Windows-basic-commands-batchscript/assets/149986612/d6c1ee8e-2a03-4066-a24a-992a0ba0080f)

List the contents of the "MyLab" directory.
## COMMAND AND OUTPUT
dir %userprofile%\Desktop\MyLab

![image](https://github.com/mithra916/Windows-basic-commands-batchscript/assets/149986612/84998b8c-a803-45a3-9178-70f45987b617)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
## COMMAND AND OUTPUT
mkdir %userprofile%\Desktop\Backup
copy MyFile.txt %userprofile%\Desktop\Backup

![image](https://github.com/mithra916/Windows-basic-commands-batchscript/assets/149986612/dc1444de-fe41-4fea-82cb-2d264d7c92a4)

![image](https://github.com/mithra916/Windows-basic-commands-batchscript/assets/149986612/d516b1c8-9951-4b19-b52b-6f96f1110ae2)

Move the "MyLab" directory to the "Documents" folder.
## COMMAND AND OUTPUT
mv Myfile.txt %userprofile%\Documents

![image](https://github.com/mithra916/Windows-basic-commands-batchscript/assets/149986612/11513cd2-9516-4c17-a95f-b09affe932ff)

## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
Modify the script to delete files with the ".docx" extension from the "Documents" folder after creating the backup.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```
## OUTPUT
![image](https://github.com/mithra916/Windows-basic-commands-batchscript/assets/149986612/420d6732-bab4-4a1d-ac4c-71807da5bdce)
# RESULT:
The commands/batch files are executed successfully.
