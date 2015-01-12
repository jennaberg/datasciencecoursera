#notes from class
##week two

* commands

	* pwd: print working directory - shows path to current directory

	* clear -  clears working screen in terminal

	* ls: list - lists out all files in current directory

	* cd: change directory - changes directory to argument directory

		just cd will move you back to your home directory

		.. will move you up one directory in your tree

	* mkdir: make directory - this will make a directory argument is directory name
	
	* touch - creates a file, argument is file name
	
	* cp: copy - takes two arguments first is file to copy second is directory where you want file copied to
	
		-r: recursive - used to move a directory (here both arguments are directories)
		
	* rm: remove sends argument to the trash (argument file name)
	
		rm -r (here -r recursive used to move a directory and its contents to the trash, argument is a directory) - with out the -r you will get a directory not empty warning
		
	* mv: move - moves file, takes two arguments first is the file, second is the directory where you want it moved. 
	
		also can be used to rename a file - here both arguments are file names
		
	* echo - prints out arguments
	
	* date - prints out the date
	
* Git: in general this is a program used to keep track of changes made to files (rough analogy is likely track changes in word)  

for example if i make changes to a file locally (e.g., through terminal or TexShop) i then add the file to my repository using command 

>  git add [filename]

then i can comment on what changes i made (following analogy add a sticky note to the word doc) using the command

> git commit -m"[description of changes]"

i can then synch the changes made locally to the copy of the repo on git hub using the command

> git push origin master 

(within the directory synched with the remote repo - and i'm pretty sure this will only work if i've synched the two correctly which is the process by which the two systems know the meaning of the arguments origin and master) [i want to add that sequence of commands to these notes later - possibly the week one notes]

* Github is a web based platform to store and share repositories 

you can change files in either and then use push or pull commands to update the two versions of the repo: push goes from local to remote, pull i haven't used yet.

