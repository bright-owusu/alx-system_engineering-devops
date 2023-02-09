# Shell Permissions
## Task 0: My name is Betty
`su` (switch user) commmand is used to change from the current user to a different user.

## Task 1: Who am I
`whoami` prints out the effective username of the current user

## Task 2: Groups
`groups` prints out all the groups the current user is part of.

## Task 3: New owner
`chown` is used to change ownership of a file to another user.  
*Syntax:* `chown new_user filename`

## Task 4: Empty!
`touch` is used to create empty files  
*Syntax:* `touch filename`

## Task 5: Execute
`chmod` is used to change the permissions of a file or directory.
*Syntax:* `chmod <options> <file>`
Command to add execute permission to the owner of the file `hello` is `chmod o+x hello`.

## Task 6: Multiple permissions
`chmod og+x,u+r hello`
The command adds execute permission to the owner and group owner, and read permission to other users, to the file `hello`.

## Task 7: Everybody!
`chmod a+x hello`
The command adds execution permission to the owner, the group owner and the other users, to the file `hello`.

## Task 8: James Bond
`chmod 007 hello`
The command sets the permission to the file hello as follows:
- Owner: no permission at all
- Group: no permission at all
- Other users: all the permissions

## Task 9: John Doe
`chmod 753 hello`
The command sets the mode of the file hello to `-rwxr-x-wx`

## Task 10: Look in the mirror
`chmod --reference=olleh hello`
This command sets the mode of the file hello the same as olleh’s mode.
