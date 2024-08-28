# Automatic-file-shorter-using-Python
Description
This script organizes files into specific folders based on their file extensions (.csv, .txt, .jpg). It first checks if the necessary folders exist and creates them if they don't. Then, it moves the files into the appropriate folders.


## Ensure that Python and necessary libraries (os, shutil) are installed. These libraries are typically included in the standard Python distribution, so no additional installation should be needed.
Usage
## To use the script, ensure you have set the following variables in your script:

path: The directory path where your files are located.
folder_name: A list of folder names that you want to create if they don't already exist.
file_name: A list of filenames that you want to organize based on their extensions.
Once the variables are set, run the script. Here’s what it does:

## Folder Creation:

The script iterates through the first three elements in the folder_name list and checks if these folders exist in the specified path.
If a folder doesn’t exist, it prints the folder path and creates the folder using os.makedirs.
File Organization:
The script iterates through each file in file_name.
If a file has a .csv, .txt, or .jpg extension and doesn’t already exist in the corresponding folder, it moves the file to the appropriate folder using shutil.move.
