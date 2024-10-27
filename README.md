# NAME: PRADEEP V
# REG NO: 212223240119
# EX-08 Windows-basic-commands-batchscript


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
![325964583-66be83b0-4044-4c7f-b5bf-38f9cfe7bc42](https://github.com/user-attachments/assets/8a3a9207-bb0b-4482-9ca6-4177e99e137d)



Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
```
cd %userprofile%\Desktop\MyLab
```
![325964712-fccf8364-6dd7-4396-bc5e-f43b42a8ff0a](https://github.com/user-attachments/assets/5d1163d8-050f-4fa4-9d31-1b3056277404)
![325964739-793e34af-fa69-4b6c-bcce-167bc8d3c9cf](https://github.com/user-attachments/assets/ced111de-0baf-47b4-b676-6e1bd156e2a9)



List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
```

dir %userprofile%\Desktop\MyLab
```

![325964850-4b74dc29-befc-416e-8286-04a31b5c1755](https://github.com/user-attachments/assets/5337c0ba-800b-488c-b65e-fffdb8304df2)


Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
```
![325964952-23d8f80d-2497-4cf2-bd1d-f6b7af312b0f](https://github.com/user-attachments/assets/4167bf2c-6c93-4d3c-aec0-6dbd37278605)

![325964977-64f3cb6f-8c8c-4168-bb17-f6a5ac8fe9c9](https://github.com/user-attachments/assets/df8e9054-a40a-44a9-922c-aad398982d1d)


Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
```

mv Myfile.txt %userprofile%\Documents
```
![325965069-43d81b74-fabc-41ee-be32-b905f7322310](https://github.com/user-attachments/assets/cd8d32aa-5df5-4650-94c0-f4da8cb5a733)

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
![325965215-3a4f96f3-07b1-4f51-afae-fe6709831448](https://github.com/user-attachments/assets/32e7079f-36ff-41a6-9676-e78d65dd7d89)





# RESULT:
The commands/batch files are executed successfully.

