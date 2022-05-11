This is Project 0x01. Shell, permissions

0-iam_betty: 			su betty
				Switches the current user to the user "betty"

1-who_am_i:			whoami
				Prints the effective username of the current user

2-groups:			groups
				Prints all the groups the current user is part of

3-new_owner:			sudo chown betty hello
				Changes the owner of the file "hello" to the user "betty"

4-empty:			touch hello
				Creates an empty file called "hello"

5-execute:			chmod u+x hello
				Adds execute permission to the owner of the file "hello"

6-multiple_permissions:		chmod ug+x,o+r hello
				Adds execute permission to the owner and the group owner, and read permission to other users, to the file "hello"

7-everybody:			chmod a+x hello
				Adds execution permission to the owner, the group owner and the other users, to the file "hello"

8-James_Bond:			chmod 007 hello
				Gives all permissions to Other users only for file "hello"

9-John_Doe:			chmod 753 hello
				Sets permissions to "rwx r-x -wx" for file "hello"

10-mirror_permissions:		chmod --reference=olleh hello
				Sets the mode of the file "hello" the same as "olleh"s mode

11-directories_permissions:	chmod a+X *
				Adds execute permission to all subdirectories of the current directory for the owner, the group owner and all other users

12-directory_permissions:	mkdir -m 751 my_dir
				Creates a directory called "my_dir" with permissions 751 in the working directory

13-change_group:		chgrp school hello
				Changes the group owner to "school" for the file "hello"

100-change_owner_and_group:	sudo chown vincent:staff .*/*
				Changes the owner to "vincent" and the group owner to "staff" for all the files and directories in the working directory

101-symbolic_link_permissions:	sudo chown -h vincent:staff _hello
				Changes the owner and the group owner of "_hello" to "vincent" and "staff" respectively

102-if_only:			sudo chown --from=guillaume vincent hello
				Changes the owner of the file "hello" to "vincent", only if it is owned by the user "guillaume"

103-Star_Wars:			telnet towel.blinkenlights.nl
				Will play the StarWars IV episode in the terminal (if telnet is installed)

