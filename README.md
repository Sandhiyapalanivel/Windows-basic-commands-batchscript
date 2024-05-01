# Windows-basic-commands-batchscript
## Ex08-Windows-basic-commands-batchscript
#### Name : SANDHIYA P
#### Register No : 212223230183
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
```
mkdir %userprofile%\Desktop\MyLab
```
![image](https://github.com/Sandhiyapalanivel/Windows-basic-commands-batchscript/assets/145743091/36936d11-8c99-4a06-86bd-371f77970536)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
```
cd %userprofile%\Desktop\MyLab
```
![image](https://github.com/Sandhiyapalanivel/Windows-basic-commands-batchscript/assets/145743091/8781dff8-8728-4e41-8a57-a93ab34f1897)

![image](https://github.com/Sandhiyapalanivel/Windows-basic-commands-batchscript/assets/145743091/099dfe54-7391-40e7-bd86-8803550fdb23)

List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
```
dir %userprofile%\Desktop\MyLab
```
![image](https://github.com/Sandhiyapalanivel/Windows-basic-commands-batchscript/assets/145743091/f052d54b-31de-4d1e-a370-f41b99ea3076)

## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.
```
mkdir %userprofile%\Desktop\Backup
copy MyFile.txt %userprofile%\Desktop\Backup
```

![image](https://github.com/Sandhiyapalanivel/Windows-basic-commands-batchscript/assets/145743091/ebce6ac2-931c-4bdb-bfd6-de038a3de91f)
![image](https://github.com/Sandhiyapalanivel/Windows-basic-commands-batchscript/assets/145743091/ce5af7b3-b94c-4b25-963e-dda2fb46b423)


## COMMAND AND OUTPUT
```
mv Myfile.txt %userprofile%\Documents
```
![image](https://github.com/Sandhiyapalanivel/Windows-basic-commands-batchscript/assets/145743091/edcc3337-11c3-4b63-9ec3-f002ca7baa58)


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


# OUTPUT

![image](https://github.com/Sandhiyapalanivel/Windows-basic-commands-batchscript/assets/145743091/6258a13c-9ddd-4789-a9b0-d9c25d79fc3f)



# RESULT:
The commands/batch files are executed successfully.

