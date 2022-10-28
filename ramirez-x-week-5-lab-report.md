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
...lots more files...
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

````
ex2
````

````

ex3
````

````

-type
<br> finds files of the type specified after it (d = directory, f = files,...)
<br> ex1
````

````
ex2
````

````

ex3
````

````
