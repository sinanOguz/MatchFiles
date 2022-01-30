# MatchFiles
Sorts and matches given files in two different directories by creation date, then writes the names of the sorted and matched files into an .xlsx file.
Multiple worksheet creation in the same .xlsx file avaliable.

# Usage
```sh
python3 matchFiles.py [path/Directory_1] [path/Directory_2][fileName][worksheetName]
```
# Example 1 -- Creating the .xlsx file for the first time
Example for video and log files of Formation_Establishment_Task

#### Directories
| Files in 'Logs/Formation_Establishment_Logs/' directory | Date of creation |
| ------ | ------ |
| 20220129192256.pkl  | Sat 29 Jan 2022 19:22:56 |
| 20220129192804.pkl | Sat 29 Jan 2022 19:28:04 |
| 20220129193334.pkl | Sat 29 Jan 2022 19:33:34|


| Files in 'Videos/Formation_Establishment_Videos/' directory | Date of creation |
| ------ | ------ |
| BB5A0872.MOV  | Sat 29 Jan 2022 19:23:01 |
| BB5A0873.MOV | Sat 29 Jan 2022 19:28:31 |
| BB5A0874.MOV | Sat 29 Jan 2022 19:35:05|

#### Command
```sh
python3 matchFiles.py  Logs/Formation_Establishment_Logs/   Videos/Formation_Establishment_Videos/   SoNS_Experiments    Formation_Establishment_Task
```
#### Result
> On the terminal screen you will see the following:
`A new spreadsheed is created.` 

![image1](https://drive.google.com/uc?export=view&id=1xkqDgYXrB-bEDgqUNM2Jb48tqDCZw1ru)

# Example 2 -- Creating a new worksheet in the same .xlsx file 
Adding the video and log files of Formation_Switching_Task into the same .xlsx file
#### Directories
| Files in 'Logs/Formation_Switching_Logs/' directory | Date of creation |
| ------ | ------ |
| 20220129192256.pkl  | Sat 29 Jan 2022 19:22:56 |
| 20220129192804.pkl | Sat 29 Jan 2022 19:28:04 |
| 20220129193334.pkl | Sat 29 Jan 2022 19:33:34|


| Files in 'Videos/Formation_Switching_Videos/' directory | Date of creation |
| ------ | ------ |
| BB5A0872.MOV  | Sat 29 Jan 2022 19:23:01 |
| BB5A0873.MOV | Sat 29 Jan 2022 19:28:31 |
| BB5A0874.MOV | Sat 29 Jan 2022 19:35:05|

#### Command
```sh
python3 matchFiles.py  Logs/Formation_Switching_Logs/   Videos/Formation_Switching_Videos/   SoNS_Experiments    Formation_Switching_Task
```
#### Result
> On the terminal screen you will see the following:
`The spreadsheet has already been created. Overwriting the spreadsheet.` 

![image2](https://drive.google.com/uc?export=view&id=1RSPbHrGeOPK87qlbxDiWlirdlq72SWbM)
