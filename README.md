# python_parse_file

# Security Log File Analysis

In this lab, I prepared a security log file for analysis and create a text file with IP addresses that are allowed to access restricted information.

## Task 1

Here, I will start by storing the file in memory.

### Steps

1. **Reset the `data/login.txt` File:**
   The script resets the `data/login.txt` file to its original contents. This allows learners to complete the lab more than once.

2. **Assign Original Contents:**
   The original contents of the file are assigned to the `login_file` variable.

   ```python
   login_file = """username,ip_address,time,date
   tshah,192.168.92.147,15:26:08,2022-05-10
   dtanaka,192.168.98.221,9:45:18,2022-05-09
   tmitchel,192.168.110.131,14:13:41,2022-05-11
   daquino,192.168.168.144,7:02:35,2022-05-08
   eraab,192.168.170.243,1:45:14,2022-05-11
   jlansky,192.168.238.42,1:07:11,2022-05-11
   acook,192.168.52.90,9:56:48,2022-05-10
   asundara,192.168.58.217,23:17:52,2022-05-12
   jclark,192.168.214.49,20:49:00,2022-05-10
   cjackson,192.168.247.153,19:36:42,2022-05-12
   jclark,192.168.197.247,14:11:04,2022-05-12
   apatel,192.168.46.207,17:39:42,2022-05-10
   mabadi,192.168.96.244,10:24:43,2022-05-12
   iuduike,192.168.131.147,17:50:00,2022-05-11
   abellmas,192.168.60.111,13:37:05,2022-05-10
   gesparza,192.168.148.80,6:30:14,2022-05-11
   cgriffin,192.168.4.157,23:04:05,2022-05-09
   alevitsk,192.168.210.228,8:10:43,2022-05-08
   eraab,192.168.24.12,11:29:27,2022-05-11
   jsoto,192.168.25.60,5:09:21,2022-05-09
   """
## Create the 'data' Directory:
The script creates the data directory to store the log file.

!mkdir -p data 
## Write login_file to data/login.txt:
The script writes the contents of login_file to the data/login.txt file.

with open("data/login.txt", "w") as file:
    file.write(login_file) 
    
# Import Security Log File:
The script imports the security log file and stores it as a string.

import_file = "data/login.txt"

with open(import_file, "r") as file:
    text = file.read()
# Display the Contents of text:
The script displays the contents of the text variable.
print(text)

## Prerequisites
Python 3.x
Basic knowledge of Python file handling
Access to a terminal or command prompt

## Usage Examples
To reset the data/login.txt file and display its contents:

Save the provided Python script to a file, e.g., reset_log.py.

Run the script in your terminal or command prompt:
python reset_log.py

## Common Issues
Ensure the data directory exists or is created by the script.
Verify the file path if running into file not found errors.
Make sure you have write permissions to the directory where the script is run.
