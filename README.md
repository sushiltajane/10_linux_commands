# 10_linux_commands

mkdir students → Creates a new directory named students.

cd students → Changes the current working directory to students.

pwd → Prints the current working directory path.

touch marks.txt names.txt → Creates empty files marks.txt and names.txt.

ls → Lists files and directories in the current location.

ls -la → Lists files with detailed information, including hidden files.

vim filename → Opens a file in the vim text editor.

cat names.txt → Displays the content of names.txt.

head -n 2 names.txt → Shows the first 2 lines of names.txt.

tail -n 2 names.txt → Shows the last 2 lines of names.txt.

wc -l names.txt → Counts the number of lines in names.txt.

sort names.txt → Sorts the lines of names.txt alphabetically.

uniq names.txt → Removes consecutive duplicate lines from names.txt.

grep "tejas" names.txt → Searches for the word tejas in names.txt.

sort names.txt | uniq → Sorts and removes duplicate lines from names.txt.


sush@LAPTOP-HO1522E5:~$ mkdir students
sush@LAPTOP-HO1522E5:~$ cd students
sush@LAPTOP-HO1522E5:~/students$ pwd
/home/sush/students
sush@LAPTOP-HO1522E5:~/students$ touch marks.txt names.txt
sush@LAPTOP-HO1522E5:~/students$ ls
marks.txt  names.txt
sush@LAPTOP-HO1522E5:~/students$ ls -la
total 8
drwxr-xr-x 2 sush sush 4096 Sep  2 06:17 .
drwxr-x--- 5 sush sush 4096 Sep  2 06:16 ..
-rw-r--r-- 1 sush sush    0 Sep  2 06:17 marks.txt
-rw-r--r-- 1 sush sush    0 Sep  2 06:17 names.txt
sush@LAPTOP-HO1522E5:~/students$ vim marks.txt
sush@LAPTOP-HO1522E5:~/students$ vim names.txt
sush@LAPTOP-HO1522E5:~/students$ cat names.txt
sushil
shreyash
tejas
om
soham
sush@LAPTOP-HO1522E5:~/students$ head -n 2 names.txt
sushil
shreyash
sush@LAPTOP-HO1522E5:~/students$ tail -n 2 names.txt
om
soham
sush@LAPTOP-HO1522E5:~/students$ wc -l names.txt
5 names.txt
sush@LAPTOP-HO1522E5:~/students$ sort names.txt
om
shreyash
soham
sushil
tejas
sush@LAPTOP-HO1522E5:~/students$ uniq names.txt
sushil
shreyash
tejas
om
soham
sush@LAPTOP-HO1522E5:~/students$ grep "tejas" names.txt
tejas
sush@LAPTOP-HO1522E5:~/students$ sort names.txt | uniq
om
shreyash
soham
sushil
tejas
