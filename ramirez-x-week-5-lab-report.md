Find Command Options

-depth
<br> looks as far down as possible into each directory before returning the directory itself
<br> ex1
````
[cs15lfa22ed@ieng6-202]:skill-demo1:210$ find technical/government/Media -depth
technical/government/Media/5_Legal_Groups.txt
technical/government/Media/AP_LawSchoolDebts.txt
technical/government/Media/A_Perk_of_Age.txt
technical/government/Media/A_helping_hand.txt
technical/government/Media/Abuse_penalties.txt
... a lot of files...
technical/government/Media/not_accessible_to_disabled.txt
technical/government/Media/predatory_loans.txt
technical/government/Media/pro_bono_efforts.txt
technical/government/Media/residents_sue_city.txt
technical/government/Media/water_fees.txt
technical/government/Media
````
ex2
````
[cs15lfa22ed@ieng6-202]:skill-demo1:211$ find technical/biomed -depth
technical/biomed/1468-6708-3-1.txt
technical/biomed/1468-6708-3-10.txt
technical/biomed/1468-6708-3-3.txt
technical/biomed/1468-6708-3-4.txt
technical/biomed/1468-6708-3-7.txt
... a lot of files ...
technical/biomed/gb-2003-4-7-r46.txt
technical/biomed/gb-2003-4-8-r50.txt
technical/biomed/gb-2003-4-8-r51.txt
technical/biomed/gb-2003-4-9-r57.txt
technical/biomed/gb-2003-4-9-r58.txt
technical/biomed/gb-2003-4-9-r60.txt
technical/biomed/rr166.txt
technical/biomed/rr167.txt
technical/biomed/rr171.txt
technical/biomed/rr172.txt
technical/biomed/rr191.txt
technical/biomed/rr196.txt
technical/biomed/rr37.txt
technical/biomed/rr73.txt
technical/biomed/rr74.txt
technical/biomed
````
ex 3
````
[cs15lfa22ed@ieng6-202]:skill-demo1:212$ find technical/plos -depth
technical/plos/journal.pbio.0020001.txt
technical/plos/journal.pbio.0020010.txt
technical/plos/journal.pbio.0020012.txt
technical/plos/journal.pbio.0020013.txt
technical/plos/journal.pbio.0020019.txt
... a lot of files ...
technical/plos/pmed.0020273.txt
technical/plos/pmed.0020274.txt
technical/plos/pmed.0020275.txt
technical/plos/pmed.0020278.txt
technical/plos/pmed.0020281.txt
technical/plos
````
-size
<br> finds files of the size specified. character suffixes change what size it is actually looking for (M = megabytes, k = kilobytes,...)
<br> ex1
````
[cs15lfa22ed@ieng6-203]:skill-demo1:214$ find technical/911report -size 1M
technical/911report
technical/911report/chapter-1.txt
technical/911report/chapter-10.txt
technical/911report/chapter-11.txt
technical/911report/chapter-12.txt
technical/911report/chapter-13.1.txt
technical/911report/chapter-13.2.txt
technical/911report/chapter-13.3.txt
technical/911report/chapter-13.4.txt
technical/911report/chapter-13.5.txt
technical/911report/chapter-2.txt
technical/911report/chapter-3.txt
technical/911report/chapter-5.txt
technical/911report/chapter-6.txt
technical/911report/chapter-7.txt
technical/911report/chapter-8.txt
technical/911report/chapter-9.txt
technical/911report/preface.txt
````
ex2
````
[cs15lfa22ed@ieng6-203]:skill-demo1:215$ find technical/plos -size 10k
technical/plos/journal.pbio.0020042.txt
technical/plos/journal.pbio.0020073.txt
technical/plos/journal.pbio.0020156.txt
technical/plos/journal.pbio.0020215.txt
technical/plos/journal.pbio.0020224.txt
technical/plos/journal.pbio.0020297.txt
technical/plos/journal.pbio.0030131.txt
technical/plos/pmed.0020005.txt
technical/plos/pmed.0020075.txt
````

ex3
````
[cs15lfa22ed@ieng6-203]:skill-demo1:217$ find technical/ -size 2k
technical/government/Media/Campaign_Pays.txt
technical/government/Media/Court_Keeps_Judge_From.txt
technical/government/Media/Fire_Victims_Sue.txt
technical/government/Media/Helping_Hands.txt
technical/government/Media/It_Pays_to_Know.txt
technical/government/Media/Justice_requests.txt
technical/government/Media/Lawyer_Web_Survey.txt
technical/government/Media/Self-Help_Website.txt
technical/government/Media/Wilmington_lawyer.txt
technical/plos/pmed.0020028.txt
technical/plos/pmed.0020048.txt
technical/plos/pmed.0020082.txt
technical/plos/pmed.0020120.txt
technical/plos/pmed.0020157.txt
technical/plos/pmed.0020192.txt
````

-type
<br> finds files of the type specified after it (d = directory, f = files,...)
<br> ex1
````
[cs15lfa22ed@ieng6-203]:skill-demo1:218$ find technical/ -type d
technical/
technical/911report
technical/biomed
technical/government
technical/government/About_LSC
technical/government/Alcohol_Problems
technical/government/Env_Prot_Agen
technical/government/Gen_Account_Office
technical/government/Media
technical/government/Post_Rate_Comm
technical/plos
````
ex2
````
[cs15lfa22ed@ieng6-203]:skill-demo1:219$ find technical/government -type d
technical/government
technical/government/About_LSC
technical/government/Alcohol_Problems
technical/government/Env_Prot_Agen
technical/government/Gen_Account_Office
technical/government/Media
technical/government/Post_Rate_Comm
````

ex3
````
[cs15lfa22ed@ieng6-203]:skill-demo1:220$ find technical/government/Media -type f
technical/government/Media/5_Legal_Groups.txt
technical/government/Media/AP_LawSchoolDebts.txt
technical/government/Media/A_Perk_of_Age.txt
technical/government/Media/A_helping_hand.txt
technical/government/Media/Abuse_penalties.txt
technical/government/Media/Advocate_for_Poor.txt
technical/government/Media/Aid_Gets_7_Million.txt
technical/government/Media/All_May_Have_Justice.txt
technical/government/Media/Annual_Fee.txt
technical/government/Media/Anthem_Payout.txt
technical/government/Media/Assuring_Underprivileged.txt
technical/government/Media/Attorney_gives_his_time.txt
technical/government/Media/Avoids_Budget_Cut.txt
technical/government/Media/Barnes_Volunteers.txt
technical/government/Media/Barnes_new_job.txt
... a lot of files ...
technical/government/Media/man_on_national_team.txt
technical/government/Media/not_accessible_to_disabled.txt
technical/government/Media/predatory_loans.txt
technical/government/Media/pro_bono_efforts.txt
technical/government/Media/residents_sue_city.txt
technical/government/Media/water_fees.txt
````
