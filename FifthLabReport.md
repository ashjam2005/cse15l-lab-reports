# CSE 15L (Fifth Lab report)
Citation: Link

In this lab, I am going to be reporting my findings on research on the ls command. There are 4 possible variations of the grep command:

-R (Lists all files recursively, descending down directory tree from given path)

-i (Gives entire information about files in long format)

-o (Same like -i but no group name)

-g (Same like -i but no owner name)


## First Type
### -R

Below is one example of "ls -R" execution. As we can see below, each file's path is listed recursively, descending down directory tree.

```
#Code block

ls -R

````

```
#Output

DocSearchServer.java  Server.java         berlitz1_sizes.txt  find-results.txt  kaufman_sizes.txt  something.txt
README.md             TestDocSearch.java  berlitz_2.txt       grep-results.txt  lib                written_2

./lib:
hamcrest-core-1.3.jar  junit-4.13.2.jar

./written_2:
count-txts.sh  find-results.txt  grep-results.txt  non-fiction  travel_guides

./written_2/non-fiction:
OUP

./written_2/non-fiction/OUP:
Abernathy  Berk  Castro  Fletcher  Kauffman  Rybczynski

./written_2/non-fiction/OUP/Abernathy:
ch1.txt  ch14.txt  ch15.txt  ch2.txt  ch3.txt  ch6.txt  ch7.txt  ch8.txt  ch9.txt  something.txt

./written_2/non-fiction/OUP/Berk:
CH4.txt  ch1.txt  ch2.txt  ch7.txt

./written_2/non-fiction/OUP/Castro:
chA.txt  chB.txt  chC.txt  chL.txt  chM.txt  chN.txt  chO.txt  chP.txt  chQ.txt  chR.txt  chV.txt  chW.txt  chY.txt  chZ.txt

./written_2/non-fiction/OUP/Fletcher:
ch1.txt  ch10.txt  ch2.txt  ch5.txt  ch6.txt  ch9.txt

./written_2/non-fiction/OUP/Kauffman:
ch1.txt  ch10.txt  ch3.txt  ch4.txt  ch5.txt  ch6.txt  ch7.txt  ch8.txt  ch9.txt

./written_2/non-fiction/OUP/Rybczynski:
ch1.txt  ch2.txt  ch3.txt

./written_2/travel_guides:
berlitz1  berlitz2

./written_2/travel_guides/berlitz1:
HandRHawaii.txt        HistoryEdinburgh.txt  HistoryLakeDistrict.txt  IntroIsrael.txt        WhatToEdinburgh.txt     WhatToLasVegas.txt    WhereToIsrael.txt
HandRHongKong.txt      HistoryEgypt.txt      HistoryLasVegas.txt      IntroIstanbul.txt      WhatToEgypt.txt         WhatToLosAngeles.txt  WhereToIstanbul.txt
HandRIbiza.txt         HistoryFWI.txt        HistoryMadeira.txt       IntroItaly.txt         WhatToFWI.txt           WhatToMadeira.txt     WhereToItaly.txt
HandRIsrael.txt        HistoryFrance.txt     HistoryMadrid.txt        IntroJamaica.txt       WhatToFrance.txt        WhatToMalaysia.txt    WhereToJapan.txt
HandRIstanbul.txt      HistoryGreek.txt      HistoryMalaysia.txt      IntroJapan.txt         WhatToGreek.txt         WhatToMallorca.txt    WhereToJerusalem.txt
HandRJamaica.txt       HistoryHawaii.txt     HistoryMallorca.txt      IntroJerusalem.txt     WhatToHawaii.txt        WhereToDublin.txt     WhereToLakeDistrict.txt
HandRJerusalem.txt     HistoryHongKong.txt   IntroDublin.txt          IntroLakeDistrict.txt  WhatToHongKong.txt      WhereToEdinburgh.txt  WhereToLosAngeles.txt
HandRLakeDistrict.txt  HistoryIbiza.txt      IntroEdinburgh.txt       IntroLasVegas.txt      WhatToIbiza.txt         WhereToEgypt.txt      WhereToMadeira.txt
HandRLasVegas.txt      HistoryIndia.txt      IntroEgypt.txt           IntroLosAngeles.txt    WhatToIndia.txt         WhereToFWI.txt        WhereToMadrid.txt
HandRLisbon.txt        HistoryIsrael.txt     IntroFWI.txt             IntroMadeira.txt       WhatToIsrael.txt        WhereToFrance.txt     WhereToMalaysia.txt
HandRLosAngeles.txt    HistoryIstanbul.txt   IntroFrance.txt          IntroMadrid.txt        WhatToIstanbul.txt      WhereToGreek.txt      WhereToMallorca.txt
HandRMadeira.txt       HistoryItaly.txt      IntroGreek.txt           IntroMalaysia.txt      WhatToItaly.txt         WhereToHawaii.txt
HandRMadrid.txt        HistoryJamaica.txt    IntroHongKong.txt        IntroMallorca.txt      WhatToJamaica.txt       WhereToHongKong.txt
HandRMallorca.txt      HistoryJapan.txt      IntroIbiza.txt           JungleMalaysia.txt     WhatToJapan.txt         WhereToIbiza.txt
HistoryDublin.txt      HistoryJerusalem.txt  IntroIndia.txt           WhatToDublin.txt       WhatToLakeDistrict.txt  WhereToIndia.txt


./written_2/travel_guides/berlitz2:
Algarve-History.txt      Bahamas-Intro.txt        Berlin-WhatToDo.txt       Canada-WhereToGo.txt         CostaBlanca-History.txt   Paris-WhatToDo.txt
Algarve-Intro.txt        Bahamas-WhatToDo.txt     Berlin-WhereToGo.txt      CanaryIslands-History.txt    CostaBlanca-WhatToDo.txt  Paris-WhereToGo.txt
Algarve-WhatToDo.txt     Bahamas-WhereToGo.txt    Bermuda-WhatToDo.txt      CanaryIslands-WhatToDo.txt   Crete-History.txt         Poland-History.txt
Algarve-WhereToGo.txt    Bali-History.txt         Bermuda-WhereToGo.txt     CanaryIslands-WhereToGo.txt  Crete-WhatToDo.txt        Poland-WhatToDo.txt
Amsterdam-History.txt    Bali-WhatToDo.txt        Bermuda-history.txt       Cancun-History.txt           Crete-WhereToGo.txt       Portugal-History.txt
Amsterdam-Intro.txt      Bali-WhereToGo.txt       Boston-WhereToGo.txt      Cancun-WhatToDo.txt          CstaBlanca-WhereToGo.txt  Portugal-WhatToDo.txt
Amsterdam-WhatToDo.txt   Barcelona-History.txt    Budapest-History.txt      Cancun-WhereToGo.txt         Cuba-History.txt          Portugal-WhereToGo.txt
Amsterdam-WhereToGo.txt  Barcelona-WhatToDo.txt   Budapest-WhatToDo.txt     China-History.txt            Cuba-WhatToDo.txt         PuertoRico-History.txt
Athens-History.txt       Barcelona-WhereToGo.txt  Budapest-WhereoGo.txt     China-WhatToDo.txt           Cuba-WhereToGo.txt        PuertoRico-WhatToDo.txt
Athens-Intro.txt         Beijing-History.txt      California-History.txt    China-WhereToGo.txt          Nepal-History.txt         PuertoRico-WhereToGo.txt
Athens-WhatToDo.txt      Beijing-WhatToDo.txt     California-WhatToDo.txt   Costa-History.txt            Nepal-WhatToDo.txt        Vallarta-History.txt
Athens-WhereToGo.txt     Beijing-WhereToGo.txt    California-WhereToGo.txt  Costa-WhatToDo.txt           Nepal-WhereToGo.txt       Vallarta-WhatToDo.txt
Bahamas-History.txt      Berlin-History.txt       Canada-History.txt        Costa-WhereToGo.txt          NewOrleans-History.txt    Vallarta-WhereToGo.txt
```

## Second Type
### -l

Below is one example of -l command. As we can see below, entire information is given about files in a long format.


```
# Code block

ls -l
```

```
#Output

-rw-r----- 1 cs15lwi23abq ieng6_cs15lwi23 2514 Feb 13 13:26 DocSearchServer.java
-rw-r----- 1 cs15lwi23abq ieng6_cs15lwi23   83 Feb 13 13:26 README.md
-rw-r----- 1 cs15lwi23abq ieng6_cs15lwi23 1890 Feb 13 13:26 Server.java
-rw-r----- 1 cs15lwi23abq ieng6_cs15lwi23  871 Feb 13 13:26 TestDocSearch.java
-rw-r----- 1 cs15lwi23abq ieng6_cs15lwi23 7601 Feb 13 13:26 berlitz1_sizes.txt
-rw-r----- 1 cs15lwi23abq ieng6_cs15lwi23 6113 Feb 13 13:26 berlitz_2.txt
-rw-r----- 1 cs15lwi23abq ieng6_cs15lwi23    0 Feb 13 13:26 find-results.txt
-rw-r----- 1 cs15lwi23abq ieng6_cs15lwi23    0 Feb 13 13:26 grep-results.txt
-rw-r----- 1 cs15lwi23abq ieng6_cs15lwi23  604 Feb 13 13:26 kaufman_sizes.txt
drwxr-s--- 2 cs15lwi23abq ieng6_cs15lwi23 4096 Feb 13 13:26 lib
-rw-r----- 1 cs15lwi23abq ieng6_cs15lwi23  551 Feb 13 13:26 something.txt
drwxr-s--- 4 cs15lwi23abq ieng6_cs15lwi23 4096 Feb 13 13:26 written_2

```


## Third Type
### -o

Below is one example of -l command. As we can see below, it is identical to -i but without group name.

```
# Code block

ls -o
```

```
#Output
-rw-r----- 1 cs15lwi23abq 2514 Feb 13 13:26 DocSearchServer.java
-rw-r----- 1 cs15lwi23abq   83 Feb 13 13:26 README.md
-rw-r----- 1 cs15lwi23abq 1890 Feb 13 13:26 Server.java
-rw-r----- 1 cs15lwi23abq  871 Feb 13 13:26 TestDocSearch.java
-rw-r----- 1 cs15lwi23abq 7601 Feb 13 13:26 berlitz1_sizes.txt
-rw-r----- 1 cs15lwi23abq 6113 Feb 13 13:26 berlitz_2.txt
-rw-r----- 1 cs15lwi23abq    0 Feb 13 13:26 find-results.txt
-rw-r----- 1 cs15lwi23abq    0 Feb 13 13:26 grep-results.txt
-rw-r----- 1 cs15lwi23abq  604 Feb 13 13:26 kaufman_sizes.txt
drwxr-s--- 2 cs15lwi23abq 4096 Feb 13 13:26 lib
-rw-r----- 1 cs15lwi23abq  551 Feb 13 13:26 something.txt
drwxr-s--- 4 cs15lwi23abq 4096 Feb 13 13:26 written_2
```

## Fourth Type
### -g

Below is one example of -g command. As we can see below, it is identical to -i but without owner name.

```
#Code block
ls -c 
```

```
#Output

-rw-r----- 1 ieng6_cs15lwi23 2514 Feb 13 13:26 DocSearchServer.java
-rw-r----- 1 ieng6_cs15lwi23   83 Feb 13 13:26 README.md
-rw-r----- 1 ieng6_cs15lwi23 1890 Feb 13 13:26 Server.java
-rw-r----- 1 ieng6_cs15lwi23  871 Feb 13 13:26 TestDocSearch.java
-rw-r----- 1 ieng6_cs15lwi23 7601 Feb 13 13:26 berlitz1_sizes.txt
-rw-r----- 1 ieng6_cs15lwi23 6113 Feb 13 13:26 berlitz_2.txt
-rw-r----- 1 ieng6_cs15lwi23    0 Feb 13 13:26 find-results.txt
-rw-r----- 1 ieng6_cs15lwi23    0 Feb 13 13:26 grep-results.txt
-rw-r----- 1 ieng6_cs15lwi23  604 Feb 13 13:26 kaufman_sizes.txt
drwxr-s--- 2 ieng6_cs15lwi23 4096 Feb 13 13:26 lib
-rw-r----- 1 ieng6_cs15lwi23  551 Feb 13 13:26 something.txt
drwxr-s--- 4 ieng6_cs15lwi23 4096 Feb 13 13:26 written_2

```
