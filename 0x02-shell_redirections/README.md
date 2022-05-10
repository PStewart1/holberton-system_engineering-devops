0-hello_world: 		echo "Hello, World"			
			A script that prints “Hello, World”, followed by a new line to the standard output

1-confused_smiley:	echo '"(Ôo)'"'" 			
			A script that displays a confused smiley

2-hellofile: 		cat /etc/passwd				
			A script to display the content of the /etc/passwd file

3-twofiles: 		cat /etc/passwd /etc/hosts		
			A script to display the content of /etc/passwd and /etc/hosts

4-lastlines: 		tail /etc/passwd 			
			A script to display the last 10 lines of /etc/passwd

5-firstlines: 		head /etc/passwd			
			A script to display the first 10 lines of /etc/passwd

6-third_line: 		head -n3 iacta | tail -n1		
			A script that displays the third line of the file iacta

7-file:			echo 'Best School' > \\\*\\\\\'"Best School"\\\'\\\\\*\$\\\?\\\*\\\*\\\*\\\*\\\*\:\)
			A script that creates a file named exactly \*\\'"Best School"\'\\*$\?\*\*\*\*\*:) containing the text Best School ending by a new line

8-cwd_state:		ls -la > ls_cwd_content
			A script that writes into the file ls_cwd_content the result of the command ls -la

9-duplicate_last_line:	tail -n1 iacta >> iacta
			A script that duplicates the last line of the file iacta

10-no_more_js: 		find -name "*.js" -type f -delete
			A script that deletes all the regular files (not the directories) with a .js extension that are present in the current directory and all its subfolders

11-directories:		find -mindepth 1 -type d -print | wc -l
			A script that counts the number of directories and sub-directories in the current directory

12-newest_files:	ls -t | head
			A script that displays the 10 newest files in the current directory

13-unique:		uniq | sort 
			A script that takes a list of words as input and prints only words that appear exactly once

14-findthatword:	grep "root" /etc/passwd
			A script that displays lines containing the pattern “root” from the file /etc/passwd

15-countthatword:	grep "bin" /etc/passwd | wc -l
			A script that displays the number of lines containing the pattern “bin” in the file /etc/passwd

16-whatsnext:		grep -A 3 "root" /etc/passwd
			A script that displays lines containing the pattern “root” and 3 lines after them in the file /etc/passwd

17-hidethisword:	grep -v "bin" /etc/passwd
			A script that displays all the lines in the file /etc/passwd that do not contain the pattern “bin”

18-lettersonly:		grep '^[[:alpha:]]' /etc/ssh/sshd_config
			A script that displays all lines of the file /etc/ssh/sshd_config starting with a letter

19-AZ:			tr Ac Ze
			A script that replaces all characters A and c from input to Z and e respectively

20-hiago:		tr -d cC
			A script that removes all letters c and C from input

21-reverse:		rev
			Created a script that reverse its input

22-users_and_homes:	cat /etc/passwd | cut -d: -f1,6 | sort
			A script that displays all users and their home directories, sorted by users
