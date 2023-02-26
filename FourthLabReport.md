# CSE 15L (Fourth Lab report)

In this lab, I will be going to detail the steps done to achieve steps 4-9 in Week 7 lab.

## Step 4 (Log into ssh account)

To log into ssh account as quick as possible we need to ensure that we don't need to type in the password since it can be quite time-consuming.




These were the steps followed:

* In local terminal, type *ssh-keygen*

* Keep pressing `enter` until computer tells you where public key been saved
  
* Type *ssh cs15lwi23___@ieng6.ucsd.edu* and press <enter>
  
* Type *mkdir ssh* and press `enter`
  
* Type exit and then press `enter`
  
* Highlight path where public key has been saved and right click 
  
* Type following statement: `scp <path to your public SSH key> cs15lwi23__@ieng6.ucsd.edu:~/.ssh/authorized_keys` and press `enter`
  
* Press `up` 4 times (assuming this is the first time you are attempting to do these steps) and then press `enter`
  
* Now you are logged in with no need to type password
  
  
  ![Image][Report4ImageOne.jpg]

## Step 5 (Clone the git repository) 
  
  
  These are steps followed:
  
  * Go to github repository and find link to be copied
  
  * Type in terminal: `git clone <link of forked repo>`
  
  * Then press `enter`

## Step 6 (Run the tests and show one of the tests is failing)
  
  These were steps followed:
  
  * Go to week 2 of lab and copy the entire sentence for compiling J-UNIT and press <enter>
  
  * Then copy the entire code for running J-UNIT tests and then right click in terminal
  
  * Before pressing `enter`, press `ctrl-W` and just type T and then press `tab`
  
  * Then press `enter`
 
## Step 7 (Amend the bug)
  
  These were steps followed:
  
  * Type `nano' and type L and then press `tab`
  
  * Press `enter`
  
  * Edit the code to include case where two letters being compared are the same and in the last while block replace index1 with index2
  
  * Press `Ctrl-O` to save and then `Ctrl-X` to exit
  
  
 ## Step 8 (Run the tests and ensure tests succeed)
  
  Do the following steps:
  
  * Keep pressing the `up` key until you find j-unit compilation line and press `enter`
  
  * Keep pressing the `up` key until you find j-unit execution line and press `enter` (no need to delete last word since you have already executed this
  command before)
  
  ## Step 9 (Push changes)
  
  Do the following steps
  
  * Type `git add ListExamples.java` and then type `git commit -m "updated"`
 
  

  
  
 
  
  
