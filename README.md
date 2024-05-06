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
![image](https://github.com/Sarishatheiveegan/Windows-basic-commands-batchscript/assets/144979465/cb2b0591-7d16-4522-87b9-bdab71ca9e12)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.

## COMMAND AND OUTPUT
cd %userprofile%\Desktop\MyLab
![image](https://github.com/Sarishatheiveegan/Windows-basic-commands-batchscript/assets/144979465/47f0de2e-cc3b-4e03-a5ad-cab5b5de75cb)
![image](https://github.com/Sarishatheiveegan/Windows-basic-commands-batchscript/assets/144979465/09bb4649-ab8c-4525-90d2-29b9ff3f2933)


List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
dir %userprofile%\Desktop\MyLab

![image](https://github.com/Sarishatheiveegan/Windows-basic-commands-batchscript/assets/144979465/f5dce67f-d5a6-449d-bd1b-6f40fa763027)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
![image](https://github.com/Sarishatheiveegan/Windows-basic-commands-batchscript/assets/144979465/8b741415-7b03-45fd-b05f-5646008c6c59)
![image](https://github.com/Sarishatheiveegan/Windows-basic-commands-batchscript/assets/144979465/871565c1-0102-478f-be1e-eac104c38cc7)


Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
mv Myfile.txt %userprofile%\Documents

![image](https://github.com/Sarishatheiveegan/Windows-basic-commands-batchscript/assets/144979465/e015a37d-477a-458b-800f-1262cced536c)


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
![Screenshot 2024-05-06 173451](https://github.com/Sarishatheiveegan/Windows-basic-commands-batchscript/assets/144979465/c9df6dc0-b567-480a-b996-c27717ebf8cf)


# RESULT:
The commands/batch files are executed successfully.

