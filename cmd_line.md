# Prep Notes
---
## Command Line
***$*** is the **shell prompt** - it appears when the terminal is ready to accept a command 

***ls*** lists the files and folders inside the currently selected folder

***pwd*** - print working directory

***cd*** - change directory

***cd ..*** - move up one directory

***mkdir*** - make directory

***touch*** *filename.txt* - creates a new file in the working directory

--

***ls -a*** - lists all contents, including hidden files and folders

***ls -l*** - lists all contents of directory in long format

***ls -t*** - orders files and directories by the time they were last modified

- ***ls -l*** : Access rights | No# hard links | Username | Group name | Size | Time/Date | Name

--
***cp*** - copies files or directories  

 - ***cp*** *text1.txt text2.txt* - copies contents of text1 into text2
 - ***cp*** *text.txt directory/* - copies text.txt into directory
 - ***cp*** *text1.txt text2.txt directory/* - copies both to directory
 - ***cp*** *dir/text.txt dir2/*  
 
***cp \**** *dir/* - copies all files in wrking directory into dir/

***cp*** *m\*.txt dir/* copies all files in wd starting with 'm' and ending '.txt'

--

***mv*** - moves files

- ***mv*** *text.txt dir/* - moves text.txt into dir/
- ***mv*** *text.txt text2.txt dir/* - moves both into /dir
- ***mv*** *text.txt text2.txt* - renames text.txt as text2.txt

--

***rm*** - deletes files and directories

- ***rm*** *text.txt* - deletes text.txt
- ***rm -r*** *dir/* - deletes directory dir and all child directories

--

**Standard input (stdin)** - information inputed into terminal through input device

**Standard output (stdout)** - information outputted after a process has run

**Standard error (stderr)** - error message outputted by a failed process

--

***echo*** *"string"* - accepts a string as stdin and echos the string back to the terminal as stdout

***>*** - redirects the stdout to a file, **overwrites all original content**

- ***echo*** *"hello"* ***>*** *hello.txt*

***cat*** - outputs the contents of a file to the terminal

- ***cat*** *hello.txt* - hello would be displayed

***>>*** - appends the stdout to the file, rather than overwriting

***<*** - takes the stdin from the right ad inputs into program on the left

 - ***cat <*** *hello.txt*

***| (pipe)*** - takes the stdout on the left and *pipes* it as a stdin to the command on right

***wc*** - outputs the number of lines, words and characters the files has

- ***cat*** *volcanoes.txt* ***| wc | cat >*** *island.txt*  
	***cat*** *islands.txt*  
	17		26		204
	
--

***sort*** - takes the stdin and orders it alphabetically for the sdout

- ***cat*** *lakes.txt* ***| sort >*** *sorted-lakes.txt*  
***cat*** *sorted-lakes.txt* - prints the list originating from *lakes.txt*

***uniq (unique)*** - filters out adjacent, duplicate lines in a file

- ***sort*** *deserts.txt* ***| uniq*** - more effective as it lists results alphabetically so all duplicates are filtered out

- ***sort*** *deserts.txt* ***| uniq >*** *uniq-deserts.txt*

--

***grep*** - **global regular expression print**, searches for files with likes that match a patern and returns the result - case sensitive

- ***grep*** *Mount mountains.txt* - searches for 'Mount' in mountains.txt

- ***grep -i*** **Mount mountains.txt** - ***-i*** makes it case insensitive

***grep -R*** - searches all files in a specified directory

***grep -Rl*** - only outputs the file names with matched result

***sed*** - **stream editor**, accepts stdin and modifies it based on an expression befpre displaying as output data

- ***sed*** *'s/snow/rain' text.txt* - replaces the first instance of snow on each line with rain

- ***sed*** *'s/snow/rain/g' text.txt* - all instances of snow will be replaced with rain

	**s**: 'substitution' - always used in sed substitution  
	**snow**: the search string  
	**rain**: the replacement string
	
--

***nano*** *hello.txt* - opens a text editor called nano and opens/creates a file called hello.txt

***ctrl + O*** - saves a file in nano

***ctrl + X*** - exits nano

***ctrl + G*** - opens a help menu

***clear*** - clears the terminal window

***nano ~/.bash_profile*** - opens the file used to store environmental settings

***alias*** *pd="pwd"* - creates a keyboard shortcut (alias). Here, typing pd would be the same as pwd

***source ~/.bash_profile*** - makes any alias available in the current session

***export*** - makes the variable to be available to all child sessions initiated from the session you are in

***export PS1****=">>"* - sets the default command prompt to >>

**USER** contains the name of the user  
**HOME** contains the path of the home directory  
**PATH** contains a list of all directories

***env*** **(environment)** - returns a list of the enrivonment variables for the current user

***env | grep*** **PATH** - stdout of ***env*** is piped to ***grep***, which searches for **PATH** and outputs it to the terminal