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
mkdir%user profile%\Dekstop\MyLab
![image](https://github.com/swathisiva212/Windows-basic-commands-batchscript/assets/155249892/368b44ac-01e2-465d-9635-8f1d9a94330e)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
cd%user profile%\Dekstop\MyLab
![image](https://github.com/swathisiva212/Windows-basic-commands-batchscript/assets/155249892/0236873f-f82f-4cf1-a180-94e5c064d337)

![image](https://github.com/swathisiva212/Windows-basic-commands-batchscript/assets/155249892/58d71075-b386-40e0-a15a-fc462590b985)
List the contents of the "MyLab" directory.

## COMMAND AND OUTPUT
dir%user profile%\Dekstop\MyLab
![image](https://github.com/swathisiva212/Windows-basic-commands-batchscript/assets/155249892/2efbd868-41ba-4df8-98f3-1954b84c2f47)
Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
mkdir%user profile%\Dekstop\Backup

copy MyFile.txt %user profile%\Dekstop\Backup
![image](https://github.com/swathisiva212/Windows-basic-commands-batchscript/assets/155249892/0b185eee-aaa6-4667-aac6-5d75a9f214ae)

![image](https://github.com/swathisiva212/Windows-basic-commands-batchscript/assets/155249892/34d13a70-650b-474f-bdd7-ef732974337f)
Move the "MyLab" directory to the "Documents" folder.

## COMMAND AND OUTPUT
mv MyFile.txt%user profile%\Dekstop\Documents
![image](https://github.com/swathisiva212/Windows-basic-commands-batchscript/assets/155249892/5f3e432a-3ceb-4df5-8a70-19f999ac7517)

## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
modify the script to delete files with ".docx" extension fron the "Documents" folder after creating the backup.
````
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
`````






## OUTPUT


![image](https://github.com/swathisiva212/Windows-basic-commands-batchscript/assets/155249892/1f1d7dad-3005-49c1-b03b-fd8cedf32eca)



# RESULT:
The commands/batch files are executed successfully.

