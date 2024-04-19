# SPSkates-Attendance
Python program to consolidate CCA club members attendance.

Steps to use program:
1. Start by downloading everything in this repo.
2. Download full list of members from SAS and rename to current data (E.g. 19 apr 2024.xlsx)
3. Make a csv file with members name and their respective admin number and name it "namesWithAdmin.csv".
4. Have CCA sessions attendance excels in the "excels" folder. Files must follow the naming convention Wed Fri Month.xlsx (E.g. 17 19 april.xlsx).
   4.1. Note that you should name the file based on which day had a session. For example:
   4.1.1. If only Wednesday had a session, the name should be Wed Month.xlsx (E.g. 17 april.xlsx)
   4.1.2. If only Friday had a session, the name should be Fri Month.xlsx (E.g. 19 april.xlsx)
   4.1.3. If both Wednesday and Friday had a session, the name should be Wed Fri Month.xlsx (E.g. 17 19 april.xlsx)
   4.2. Do also note that the month should not be capitalised.
5. Once all these steps are done, go into the "code" folder and open the "constants.json" file
6. In there, make changes to the follow lines:
   6.1. Change the start date of the first semester. Only make changes to the numbers. For example, Semester one starts on 15 april 2024, ""SEM_1_DAY": 17," should be changed to ""SEM_1_DAY": 15," and ""SEM_1_YEAR" : 2023," should be changed to ""SEM_1_YEAR" : 2024,"
   6.2. Do the same for the second semester.
   6.3. Change the "NAME", "ADMIN_NUMBER", and "AY" to correctly reflect your name, admin number and AY.
   6.4. Change "LASTEST_NAMELIST" to the name of the SAS file (step 2) (E.g. "LASTEST_NAMELIST" : "../<19 apr>.xlsx",)
   6.5. (Optional) Change the list of exco members name under the "EXCOS" line. The format of the list should be ["Name 1", "Name 2",...]
   6.5.1. Note that there is no need to change the name unless you would like the program to show you the exco memeber's individual attenance.
   6.5.2 If you would like that to be the case, Change the value of "SHOW_EXCO_ATTENDANCE" to "true"
7. Once all these changes have been made, open a command line to the "code" folder. (If you are unsure of how to do that, follow this guide https://www.lifewire.com/open-command-prompt-in-a-folder-5185505)
8. Type "consolidate.exe" and press Enter and let the program run.
    8.1. One thing to note before running the program is that none of the files should be open. Otherwise the program will crash.
    8.2. A file named "CCA Attendance Sheet.xlsx" will be created. This files shows the consolidated attendance of each member and which day(s) they attended.
    8.3. 2 more files named "AY<your AY> S1 SD-FRM-022A CCA Records Form.docx" and "AY<your AY> S2 SD-FRM-022A CCA Records Form.docx" will be created. This are the file to be submitted to your SD officer.
9. Should there be an error go the the "Issues" tab of this repository and create a thread and I will try to reply as soon as possible.
10. That is all. If you are unsure of anything, ask your senior as they should know what to do.


   
