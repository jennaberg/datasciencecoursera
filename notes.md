#notes from class
## week one

this week i set up github account and installed the various software (git, R, Rstudio)

here i also learned how to make and connect repositories flipping back through my terminal commands i think the following sequence of commands will do what i want

* start by making the directories (one local and one on github) that you want to have connected

> click through and initialize with README.md on github

> mkdir [repo name]

* then move into the directory locally and initialize and connect to remote repo

> cd [repo name]
>  git init 
> git remote add origin [https link for github repo]


(ok i'm going to try that sequence now to see if it works) 

(that totally didn't work)

#way to connect local repo to github repo.

* make repo on git hub
* in directory one up from where you want your repo use command
> git clone [url of github repo]

i think that may be it - again i'm gong to try it to see if i need to do any init or remote stupid locally

this (above) works





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

#Adding : seems like git add -A adds all files and updates tracking for files that were changed

after adding you can commit them locally

git commit -m "useful description of changes in this commit - may refer to changes in lots of files"

to put up on github 

git push (within the directory you want to update)

#Branching

*create a new branch using command git checkout -b NAMEof branch you want to do 

( i don't know if this means create the name of new branch or if it takes as an input the thing you are branching) 


* git branch tells you which branch you are on (traditional is master)

*git checkout master will return you to the master branch

#Pull requests

(follow instructions on Github - this is a githuib, not command line operation) 

# git/github help

*http://git-smc.com/doc

*https://help.github.com

* google or stack overflow 

* Github is a web based platform to store and share repositories 

you can change files in either and then use push or pull commands to update the two versions of the repo: push goes from local to remote, pull i haven't used yet.


## week 3 (conceptual issues) 

#types of questions

* descriptive, exploratory, inferential, predictive, causal, mechanistic

* descriptive: just say what is there separate from inferring 

* exploratory: trying to find relationships (not necessarily confirm them) good for forming questions (find correlations - not causations)

* inferential: use a small amount of data and make a statement about a bigger population. involves estimation and level of uncertainty

*prediction analysis: use data on some objects to predict values on next object that you encounter (note prediction is not the same as causation)  (more data and a simple model is better) 

* causal analysis: this is very hard.  requires a randomized studies (control trials) 

*mechanistic: rarely the goal. want to understand exact changes in one variable that lead to changes in another variable (better in physical.engineering studies) 


# what is data

* data are values of qualitative or quantitative variables belonging to a set of items

** set of items : population
**variables: characteristic of  an item
**qualitative: not neck ordered or measured
** quant: usually numeric definitely order able

*what do data look like?: yuky - usually very poorly structured - not the pretty excel file that you are thinking of.

*first important item is question - then the data. (this is important) 

# what about big data

*depends on your perspective. we can collect much more data now, than we could 40 years ago (chain letter analogy) 

*big data isn't the issue - it is wether it is useful.


#experimental design 

* make a good plan (including the statistical method you want to use), 
*have a plan for sharing your data
*START WITH A QUESTION
*example of inferential statistics (using the text change donation study) 
*issue of confounding variable (shoe size and literacy example) 
* fix confounding: fix some variables, stratify (separate out data when variable isn't fixed), randomize variables that aren't fixable (explains why randomization helps) 
* prediction: terms (connecting probabilities and the quadrant of possibilities in prediction)
** sensitivity probability that if you have a positive test, given that you have the disease
**specificity: probability that you have a neg test, given that you don't have the disease
**pos predictive value: probability that you have the disease,, given that you have a positive test
**negative predictive value: probability that you don't have the disease if you have a negative test
**accuracy: probability of correct outcome
*(dude does a summary that is not what he talked about in video - odd)
**good experiments are:replicable, measure variability in replication, generalize to a problem you care about, are transparent. (note prediction and inference are different things (both important)