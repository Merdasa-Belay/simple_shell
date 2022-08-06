0x16.c - simple shell
this project is about simple UNIX command interpreter based on bash and Sh.
To start, compile all .c located in this repository by using this command:

gcc -Wall -Werror -Wextra -pedantic -std=gnu89 *.c -o hsh
Testing 
your shell should work like this in interactive mode:

$./hsh
($)/bin/ls
hsh main.c shell.c
($)
($)exit
$
but also in non-interactive mode:

$echo "/bin/ls" |./hsh
hsh main.c shell.c test_ls_2
$
$cat test_ls_2
/bin/ls
/bin/ls
$
$cat test_ls_2 | ./hsh
hsh main.c shell.c test_ls_2
hsh main.c shell.c test_ls_2
$
