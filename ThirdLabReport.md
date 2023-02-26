# CSE 15L (Third Lab report)

In this lab, I am going to be reporting my findings on research on the grep command. There are 4 possible variations of the grep command: 

* grep "some string" <name of .txt file>
  
* -v (Trying to find the lines which do not have a certain string)
  
* -n (Trying to find line numbers which contain a certain string)
  
* -c (Trying to find number of occurences of a certain string in a .txt file)
  
  
## First type
### grep "some string" <name of .txt file>
  
  
This type of grep gives an output which shows all lines that have "some string" word in the line. Below are two examples.
  
  ```
# First code block example
grep "WhatToDo" find-results.txt
```
This is the output you receive when trying to find the number of lines which have "WhatToDo" in the find-results.txt file.
  
```
  # Output
travel_guides/berlitz2/Algarve-WhatToDo.txt
travel_guides/berlitz2/Amsterdam-WhatToDo.txt
travel_guides/berlitz2/Athens-WhatToDo.txt
travel_guides/berlitz2/Bahamas-WhatToDo.txt
travel_guides/berlitz2/Bali-WhatToDo.txt
travel_guides/berlitz2/Barcelona-WhatToDo.txt
travel_guides/berlitz2/Beijing-WhatToDo.txt
travel_guides/berlitz2/Berlin-WhatToDo.txt
travel_guides/berlitz2/Bermuda-WhatToDo.txt
travel_guides/berlitz2/Budapest-WhatToDo.txt
travel_guides/berlitz2/California-WhatToDo.txt
travel_guides/berlitz2/CanaryIslands-WhatToDo.txt
travel_guides/berlitz2/Cancun-WhatToDo.txt
travel_guides/berlitz2/China-WhatToDo.txt
travel_guides/berlitz2/Costa-WhatToDo.txt
travel_guides/berlitz2/CostaBlanca-WhatToDo.txt
travel_guides/berlitz2/Crete-WhatToDo.txt
travel_guides/berlitz2/Cuba-WhatToDo.txt
travel_guides/berlitz2/Nepal-WhatToDo.txt
travel_guides/berlitz2/Paris-WhatToDo.txt
travel_guides/berlitz2/Poland-WhatToDo.txt
travel_guides/berlitz2/Portugal-WhatToDo.txt
travel_guides/berlitz2/PuertoRico-WhatToDo.txt
travel_guides/berlitz2/Vallarta-WhatToDo.txt
```

Below is second example.
  
  ```
# Second code block
grep "History" find-results.txt
```
  
This is the output you receive when trying to find the number of files which are part of berlitz 1 in the find-results.txt file.
  
```
# Output
travel_guides/berlitz1
travel_guides/berlitz1/HandRHawaii.txt
travel_guides/berlitz1/HandRHongKong.txt
travel_guides/berlitz1/HandRIbiza.txt
travel_guides/berlitz1/HandRIsrael.txt
travel_guides/berlitz1/HandRIstanbul.txt
travel_guides/berlitz1/HandRJamaica.txt
travel_guides/berlitz1/HandRJerusalem.txt
travel_guides/berlitz1/HandRLakeDistrict.txt
travel_guides/berlitz1/HandRLasVegas.txt
travel_guides/berlitz1/HandRLisbon.txt
travel_guides/berlitz1/HandRLosAngeles.txt
travel_guides/berlitz1/HandRMadeira.txt
travel_guides/berlitz1/HandRMadrid.txt
travel_guides/berlitz1/HandRMallorca.txt
travel_guides/berlitz1/HistoryDublin.txt
travel_guides/berlitz1/HistoryEdinburgh.txt
travel_guides/berlitz1/HistoryEgypt.txt
travel_guides/berlitz1/HistoryFrance.txt
travel_guides/berlitz1/HistoryFWI.txt
travel_guides/berlitz1/HistoryGreek.txt
travel_guides/berlitz1/HistoryHawaii.txt
travel_guides/berlitz1/HistoryHongKong.txt
travel_guides/berlitz1/HistoryIbiza.txt
travel_guides/berlitz1/HistoryIndia.txt
travel_guides/berlitz1/HistoryIsrael.txt
travel_guides/berlitz1/HistoryIstanbul.txt
travel_guides/berlitz1/HistoryItaly.txt
travel_guides/berlitz1/HistoryJamaica.txt
travel_guides/berlitz1/HistoryJapan.txt
travel_guides/berlitz1/HistoryJerusalem.txt
travel_guides/berlitz1/HistoryLakeDistrict.txt
travel_guides/berlitz1/HistoryLasVegas.txt
travel_guides/berlitz1/HistoryMadeira.txt
travel_guides/berlitz1/HistoryMadrid.txt
travel_guides/berlitz1/HistoryMalaysia.txt
travel_guides/berlitz1/HistoryMallorca.txt
travel_guides/berlitz1/IntroDublin.txt
travel_guides/berlitz1/IntroEdinburgh.txt
travel_guides/berlitz1/IntroEgypt.txt
travel_guides/berlitz1/IntroFrance.txt
travel_guides/berlitz1/IntroFWI.txt
travel_guides/berlitz1/IntroGreek.txt
travel_guides/berlitz1/IntroHongKong.txt
travel_guides/berlitz1/IntroIbiza.txt
travel_guides/berlitz1/IntroIndia.txt
travel_guides/berlitz1/IntroIsrael.txt
travel_guides/berlitz1/IntroIstanbul.txt
travel_guides/berlitz1/IntroItaly.txt
travel_guides/berlitz1/IntroJamaica.txt
travel_guides/berlitz1/IntroJapan.txt
travel_guides/berlitz1/IntroJerusalem.txt
travel_guides/berlitz1/IntroLakeDistrict.txt
travel_guides/berlitz1/IntroLasVegas.txt
travel_guides/berlitz1/IntroLosAngeles.txt
travel_guides/berlitz1/WhereToMadeira.txt
travel_guides/berlitz1/WhereToMadrid.txt
travel_guides/berlitz1/WhereToMalaysia.txt
travel_guides/berlitz1/WhereToMallorca.txt
```
 
  
## Second type
### grep -v "some string" <name of .txt file>
  
This type of grep command is responsible for finding the lines which do not contain a certain string. Below are two code examples and their respective outputs.

  
  ```
# First code block
grep -v "WhereTo" find results-txt
```
This is the output you receive when trying to find the number of files which do not have WhereTo in their path in the find-results.txt file.
  
```
# Output
travel_guides
travel_guides/berlitz1
travel_guides/berlitz1/HandRHawaii.txt
travel_guides/berlitz1/HandRHongKong.txt
travel_guides/berlitz1/HandRIbiza.txt
travel_guides/berlitz1/HandRIsrael.txt
travel_guides/berlitz1/HandRIstanbul.txt
travel_guides/berlitz1/HandRJamaica.txt
travel_guides/berlitz1/HandRJerusalem.txt
travel_guides/berlitz1/HandRLakeDistrict.txt
travel_guides/berlitz1/HandRLasVegas.txt
travel_guides/berlitz1/HandRLisbon.txt
travel_guides/berlitz1/HandRLosAngeles.txt
travel_guides/berlitz1/HandRMadeira.txt
travel_guides/berlitz1/HandRMadrid.txt
travel_guides/berlitz1/HandRMallorca.txt
travel_guides/berlitz1/HistoryDublin.txt
travel_guides/berlitz1/HistoryEdinburgh.txt
travel_guides/berlitz1/HistoryEgypt.txt
travel_guides/berlitz1/HistoryFrance.txt
travel_guides/berlitz1/HistoryFWI.txt
travel_guides/berlitz1/HistoryGreek.txt
travel_guides/berlitz1/HistoryHawaii.txt
travel_guides/berlitz1/HistoryHongKong.txt
travel_guides/berlitz1/HistoryIbiza.txt
travel_guides/berlitz1/HistoryIndia.txt
travel_guides/berlitz1/HistoryIsrael.txt
travel_guides/berlitz1/HistoryIstanbul.txt
travel_guides/berlitz1/HistoryItaly.txt
travel_guides/berlitz1/HistoryJamaica.txt
travel_guides/berlitz1/HistoryJapan.txt
travel_guides/berlitz1/HistoryJerusalem.txt
travel_guides/berlitz1/HistoryLakeDistrict.txt
travel_guides/berlitz1/HistoryLasVegas.txt
travel_guides/berlitz1/HistoryMadeira.txt
travel_guides/berlitz1/HistoryMadrid.txt
travel_guides/berlitz1/HistoryMalaysia.txt
travel_guides/berlitz1/HistoryMallorca.txt
travel_guides/berlitz1/IntroDublin.txt
travel_guides/berlitz1/IntroEdinburgh.txt
travel_guides/berlitz1/IntroEgypt.txt
travel_guides/berlitz1/IntroFrance.txt
travel_guides/berlitz1/IntroFWI.txt
travel_guides/berlitz1/IntroGreek.txt
travel_guides/berlitz1/IntroHongKong.txt
travel_guides/berlitz1/IntroIbiza.txt
travel_guides/berlitz1/IntroIndia.txt
travel_guides/berlitz1/IntroIsrael.txt
travel_guides/berlitz1/IntroIstanbul.txt
travel_guides/berlitz1/IntroItaly.txt
travel_guides/berlitz1/IntroJamaica.txt
travel_guides/berlitz1/IntroJapan.txt
travel_guides/berlitz1/IntroJerusalem.txt
travel_guides/berlitz1/IntroLakeDistrict.txt
travel_guides/berlitz1/IntroLasVegas.txt
travel_guides/berlitz1/IntroLosAngeles.txt
travel_guides/berlitz1/IntroMadeira.txt
travel_guides/berlitz1/IntroMadrid.txt
travel_guides/berlitz1/IntroMalaysia.txt
travel_guides/berlitz1/IntroMallorca.txt
travel_guides/berlitz1/JungleMalaysia.txt
travel_guides/berlitz1/WhatToDublin.txt
travel_guides/berlitz1/WhatToEdinburgh.txt
travel_guides/berlitz1/WhatToEgypt.txt
travel_guides/berlitz1/WhatToFrance.txt
travel_guides/berlitz1/WhatToFWI.txt
travel_guides/berlitz1/WhatToGreek.txt
  travel_guides/berlitz1/WhatToHawaii.txt
travel_guides/berlitz1/WhatToHongKong.txt
travel_guides/berlitz1/WhatToIbiza.txt
travel_guides/berlitz1/WhatToIndia.txt
travel_guides/berlitz1/WhatToIsrael.txt
travel_guides/berlitz1/WhatToIstanbul.txt
travel_guides/berlitz1/WhatToItaly.txt
travel_guides/berlitz1/WhatToJamaica.txt
travel_guides/berlitz1/WhatToJapan.txt
travel_guides/berlitz1/WhatToLakeDistrict.txt
travel_guides/berlitz1/WhatToLasVegas.txt
travel_guides/berlitz1/WhatToLosAngeles.txt
travel_guides/berlitz1/WhatToMadeira.txt
travel_guides/berlitz1/WhatToMalaysia.txt
travel_guides/berlitz1/WhatToMallorca.txt
travel_guides/berlitz2
travel_guides/berlitz2/Algarve-History.txt
travel_guides/berlitz2/Algarve-Intro.txt
travel_guides/berlitz2/Algarve-WhatToDo.txt
travel_guides/berlitz2/Amsterdam-History.txt
travel_guides/berlitz2/Amsterdam-Intro.txt
travel_guides/berlitz2/Amsterdam-WhatToDo.txt
travel_guides/berlitz2/Athens-History.txt
travel_guides/berlitz2/Athens-Intro.txt
travel_guides/berlitz2/Athens-WhatToDo.txt
travel_guides/berlitz2/Bahamas-History.txt
travel_guides/berlitz2/Bahamas-Intro.txt
travel_guides/berlitz2/Bahamas-WhatToDo.txt
travel_guides/berlitz2/Bali-History.txt
travel_guides/berlitz2/Bali-WhatToDo.txt
travel_guides/berlitz2/Barcelona-History.txt
travel_guides/berlitz2/Barcelona-WhatToDo.txt
travel_guides/berlitz2/Beijing-History.txt
travel_guides/berlitz2/Beijing-WhatToDo.txt
  travel_guides/berlitz2/Berlin-History.txt
travel_guides/berlitz2/Berlin-WhatToDo.txt
travel_guides/berlitz2/Bermuda-history.txt
travel_guides/berlitz2/Bermuda-WhatToDo.txt
travel_guides/berlitz2/Budapest-History.txt
travel_guides/berlitz2/Budapest-WhatToDo.txt
travel_guides/berlitz2/Budapest-WhereoGo.txt
travel_guides/berlitz2/California-History.txt
travel_guides/berlitz2/California-WhatToDo.txt
travel_guides/berlitz2/Canada-History.txt
travel_guides/berlitz2/CanaryIslands-History.txt
travel_guides/berlitz2/CanaryIslands-WhatToDo.txt
travel_guides/berlitz2/Cancun-History.txt
travel_guides/berlitz2/Cancun-WhatToDo.txt
travel_guides/berlitz2/China-History.txt
travel_guides/berlitz2/China-WhatToDo.txt
travel_guides/berlitz2/Costa-History.txt
travel_guides/berlitz2/Costa-WhatToDo.txt
travel_guides/berlitz2/CostaBlanca-History.txt
travel_guides/berlitz2/CostaBlanca-WhatToDo.txt
travel_guides/berlitz2/Crete-History.txt
travel_guides/berlitz2/Crete-WhatToDo.txt
travel_guides/berlitz2/Cuba-History.txt
travel_guides/berlitz2/Cuba-WhatToDo.txt
travel_guides/berlitz2/Nepal-History.txt
travel_guides/berlitz2/Nepal-WhatToDo.txt
travel_guides/berlitz2/NewOrleans-History.txt
travel_guides/berlitz2/Paris-WhatToDo.txt
travel_guides/berlitz2/Poland-History.txt
travel_guides/berlitz2/Poland-WhatToDo.txt
travel_guides/berlitz2/Portugal-History.txt
travel_guides/berlitz2/Portugal-WhatToDo.txt
travel_guides/berlitz2/PuertoRico-History.txt
travel_guides/berlitz2/PuertoRico-WhatToDo.txt
travel_guides/berlitz2/Vallarta-History.txt
travel_guides/berlitz2/Vallarta-WhatToDo.txt
    
```
  
Below is second code example.
  
  ```
# Second code block
grep -v ".txt" find-results.txt
```
This is the output when trying to find the amount of non-".txt" files in find-results.txt file. 
    
```
# Output
travel_guides
travel_guides/berlitz1
travel_guides/berlitz2
```
 
## Third type
### grep -n "some string" <name of .txt file>
   
This is responsible for stating the line numbers where a certain string exists. Below are two examples illustrating the effect.
  
```
# First code block
  grep -n "Poland" find-results.txt
```
 
Below is the output that is printed out when above code block is executed.
  
```
# Output
  
172:travel_guides/berlitz2/Poland-History.txt
173:travel_guides/berlitz2/Poland-WhatToDo.txt
``` 
  
Below is second code example.
  
 ```
# Second code block
  
  grep -n "History" find-results.txt
``` 
  
 Below is the output that is printed out when above code block is executed.
  
  ```  
#Output
17:travel_guides/berlitz1/HistoryDublin.txt
18:travel_guides/berlitz1/HistoryEdinburgh.txt
19:travel_guides/berlitz1/HistoryEgypt.txt
20:travel_guides/berlitz1/HistoryFrance.txt
21:travel_guides/berlitz1/HistoryFWI.txt
22:travel_guides/berlitz1/HistoryGreek.txt
23:travel_guides/berlitz1/HistoryHawaii.txt
24:travel_guides/berlitz1/HistoryHongKong.txt
25:travel_guides/berlitz1/HistoryIbiza.txt
26:travel_guides/berlitz1/HistoryIndia.txt
27:travel_guides/berlitz1/HistoryIsrael.txt
28:travel_guides/berlitz1/HistoryIstanbul.txt
29:travel_guides/berlitz1/HistoryItaly.txt
30:travel_guides/berlitz1/HistoryJamaica.txt
31:travel_guides/berlitz1/HistoryJapan.txt
32:travel_guides/berlitz1/HistoryJerusalem.txt
33:travel_guides/berlitz1/HistoryLakeDistrict.txt
34:travel_guides/berlitz1/HistoryLasVegas.txt
35:travel_guides/berlitz1/HistoryMadeira.txt
36:travel_guides/berlitz1/HistoryMadrid.txt
37:travel_guides/berlitz1/HistoryMalaysia.txt
38:travel_guides/berlitz1/HistoryMallorca.txt
105:travel_guides/berlitz2/Algarve-History.txt
109:travel_guides/berlitz2/Amsterdam-History.txt
113:travel_guides/berlitz2/Athens-History.txt
117:travel_guides/berlitz2/Bahamas-History.txt
121:travel_guides/berlitz2/Bali-History.txt
124:travel_guides/berlitz2/Barcelona-History.txt
127:travel_guides/berlitz2/Beijing-History.txt
130:travel_guides/berlitz2/Berlin-History.txt
137:travel_guides/berlitz2/Budapest-History.txt
140:travel_guides/berlitz2/California-History.txt
143:travel_guides/berlitz2/Canada-History.txt
145:travel_guides/berlitz2/CanaryIslands-History.txt
148:travel_guides/berlitz2/Cancun-History.txt
151:travel_guides/berlitz2/China-History.txt
154:travel_guides/berlitz2/Costa-History.txt
157:travel_guides/berlitz2/CostaBlanca-History.txt
159:travel_guides/berlitz2/Crete-History.txt
163:travel_guides/berlitz2/Cuba-History.txt
166:travel_guides/berlitz2/Nepal-History.txt
169:travel_guides/berlitz2/NewOrleans-History.txt
172:travel_guides/berlitz2/Poland-History.txt
174:travel_guides/berlitz2/Portugal-History.txt
177:travel_guides/berlitz2/PuertoRico-History.txt
180:travel_guides/berlitz2/Vallarta-History.txt
```

## Fourth type
### grep -c <name of .txt file>

This is responsible for stating the number of times a string appears in a text file. Below are two examples illustrating the effect.
  
  
```
# First code block (Responsible for returning number of .txt extensions in find-result.txt file)
grep -c ".txt" find-results.txt
```
  
 Below is the output. 
  ```
# Output
179
```
  
 Below is the second code example. 
  
  ```
# Second code block
grep -c "History" find-results.txt
```
  
 Below is the output. 
  
  ```
# code block
46
```
