# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

# AIM:
To execute Windows basic commands and batch scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Windows environment installed on the system or installed inside a virtual environment like virtual box/vmware 

### Step 2:

Write the Windows commands / batch file . Save each script in a file with a .bat extension. Ensure you have the necessary permissions to perform the operations. Adapt paths as needed based on your system configuration.
### Step 3:

Execute the necessary commands/batch file for the desired output. 
# WINDOWS COMMANDS:
## Exercise 1: Basic Directory and File Operations
Create a directory named "my-folder"
```
mkdir %userprofile%\Desktop\MyLab
```
![image](https://github.com/user-attachments/assets/fd2d326c-f1ba-4dad-b9d7-c55bb2ec299d)

## COMMAND AND OUTPUT
Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.

## COMMAND AND OUTPUT
List the contents of the "MyLab" directory.
```
cd %userprofile%\Desktop\MyLab
```
![image](https://github.com/user-attachments/assets/e4bfc3ed-8a90-45d6-88ea-d52c4b521802)
![image](https://github.com/user-attachments/assets/e67aba7c-98a1-4c49-9c0d-db70774b1955)

## COMMAND AND OUTPUT
Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
```
dir %userprofile%\Desktop\MyLab
```
![image](https://github.com/user-attachments/assets/2636f608-2fe4-4a37-a54f-8dfd66a489e1)

## COMMAND AND OUTPUT
Move the "MyLab" directory to the "Documents" folder.
```
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
```
![image](https://github.com/user-attachments/assets/705228ff-697e-426f-a46f-6382d2274d6e)
![image](https://github.com/user-attachments/assets/110411d6-84d1-42de-acf1-8bec4af23015)

## COMMAND AND OUTPUT
```
mv Myfile.txt %userprofile%\Documents
```
![WhatsApp Image 2025-05-18 at 21 07 05_6f153f16](https://github.com/user-attachments/assets/a84632ba-76b2-462b-8dfe-11b12422a999)

## Exercise 2: Advanced Batch Scripting
Create a batch file named on the desktop. The batch file need to have a variable assigned with a desired name for ex. name="John" and display as "Hello, John".
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
![image](https://github.com/user-attachments/assets/159d2f85-38cb-4a97-be4f-0d4b0eb6fe79)

# RESULT:
The commands/batch files are executed successfully.

