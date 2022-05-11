This is Project 0x00-Shell, Basics

0-current_working_directory:	pwd
				Prints the current working directory

1-listit:			ls
				List contents of current directory

2-bring_me_home:		cd /root
				Changes working directory to home directory

3-listfiles:			ls -l
				Displays current directory in long format

4-listmorefiles:		ls -la
				Displays current directory in long format, including hidden files

5-listfilesdigitonly:		ls -lan
				Displays current directory in long format, with numeric IDs, including hidden files

6-firstdirectory:		mkdir /tmp/my_first_directory
				Creates a directory "my_first_directory" in the "tmp" folder

7-movethatfile:			mv /tmp/betty /tmp/my_first_directory
				Move file "betty" to "/tmp/my_first_directory"

8-firstdelete:			rm /tmp/my_first_directory/betty
				Deletes file "betty"

9-firstdirdeletion:		rmdir /tmp/my_first_directory
				Deletes folder "my_first_directory" 

10-back:			cd -
				Change back to previous directory 

11-lists:			ls -la . .. /boot
				Lists ALL files, in long, for current directory, parent directory, and "/boot"

12-file_type:			file /tmp/iamafile
				Prints the type of file for "/tmp/iamafile"

13-symbolic_link:		ln -s /bin/ls __ls__
				Creates a "soft" symbolic link "__ls__" referencing file "/bin/ls"

14-copy_html:			cp -u *.html ..
				Copies all new html files to parent directory 

103-commas:			ls -map
				Lists all files and folders, with a specific format 
