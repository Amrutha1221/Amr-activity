# Amr-activity
activity 1
part 1
man ls -

1. ls -a

Description:Lists all files including hidden files(those starting with.).
Output:

$ ls -a
.   ..    file1.txt
file2.c     .hiddenfile

Remark:Useful to see hidden files like .gitignore or config files.


---

2. ls -b

Description:Prints non-printable characters in file names as escape sequences(/xxx).
Output:

$ ls -b
file1.txt file2\ n.txt file3.c

Remark:Helpful if filename have spaces/newlines or special chars.


---

3. ls -c

Descripton:Sorts files by last modification time,or with -l shows ctime.
Output:

$ ls -lc 
-rw-r--r--  1 user user 245 Aug 25
08:00 file2.c
-rw-r--r--  1 user user 120 Aug 24
21:12 file1.txt

Remark:Useful for checking which files were most recently changed.


---

4. ls -d

Description:Displays directories themselves,not their contents.
Output:

$ ls -d Documents/
Documents/

Remark:Helps when you only want directory names,not the files inside.


---

5. ls -e

Decription:Shows extended attributes of files(not supported everywhere).
Output:

$ ls -le
-rw-r--r--+  1 user user 245 Aug 25
08:00 file2.c

Remark:Shows extra metadata like ACLs.


---

6. ls -f

Description:Lists all files without sorting(implies -a).
Output:

$ ls -f
.  ..   file1.txt  file2.c   .hiddenfile

Remark:Fast for scripting since it skips sorting.


---

7. ls -g

Description:Like -l but hides owner information.
Output:

$ ls -lg
-rw-r--r--  1  245 Aug 25 08:00 
file2.c

Remark:Shows group but not owner.


---

8. Command: ls -h

Description: Shows file sizes in human-readable format (KB, MB).
Output:

$ ls -lh
-rw-r--r--  1 user user  12K Aug 25 08:00 file2.c

Remarks: Easier to understand file sizes.


---

9. Command: ls -i

Description: Shows inode numbers of files.
Output:

$ ls -i
123456 file1.txt   123457 file2.c

Remarks: Useful for identifying files by inode.


---

10. Command: ls -l

Description: Long listing with permissions, owner, group, size, date, and filename.
Output:

$ ls -l
-rw-r--r--  1 user user  245 Aug 25 08:00 file2.c

Remarks: Most commonly used detailed view.


---

11. Command: ls -m

Description: Lists files separated by commas.
Output:

$ ls -m
file1.txt, file2.c, file3.cpp

Remarks: Easier for single-line display.


---

12. Command: ls -n

Description: Like -l but shows numeric UID and GID.
Output:

$ ls -n
-rw-r--r--  1 1000 1000 245 Aug 25 08:00 file2.c

Remarks: Helpful when usernames/groups are not resolved.


---

13. Command: ls -o

Description: Like -l but excludes group info.
Output:

$ ls -lo
-rw-r--r--  1 user   245 Aug 25 08:00 file2.c

Remarks: Compact long listing without group info.


---

14. Command: ls -p

Description: Adds / at the end of directory names.
Output:

$ ls -p
file1.txt  file2.c  Documents/

Remarks: Useful to distinguish files from directories.


---

15. Command: ls -q

Description: Replaces non-printable characters with ?.
Output:

$ ls -q
file1.txt   file2?.txt

Remarks: Helps avoid terminal issues with weird characters.


---

16. Command: ls -r

Description: Reverses the sort order.
Output:

$ ls -r
file3.c   file2.c   file1.txt

Remarks: Lists files in reverse order.


---

17. Command: ls -s

Description: Shows file size in blocks.
Output:

$ ls -s
12 file1.txt   8 file2.c

Remarks: Useful to check disk usage.


---

18. Command: ls -t

Description: Sorts files by modification time.
Output:

$ ls -lt
-rw-r--r--  file2.c
-rw-r--r--  file1.txt

Remarks: Newest files appear first.


---

19. Command: ls -u

Description: Sorts by access time (atime).
Output:

$ ls -lu
-rw-r--r--  accessed Aug 25 file1.txt

Remarks: Helps track last accessed files.


---

20. Command: ls -v

Description: Sorts files in natural version order.
Output:

$ ls -v
file1 file2 file10

Remarks: Numbers are sorted properly (1,2,10) not alphabetically.


---

21. Command: ls -w

Description: Sets output width (default = terminal width).
Output:

$ ls -w 40
file1.txt file2.c file3.cpp ...

Remarks: Controls formatting of columns.


---

22. Command: ls -x

Description: Lists files in columns (row-wise).
Output:

$ ls -x
file1.txt file2.c file3.cpp
file4.txt file5.c

Remarks: Compact view.


---

23. Command: ls -y

Description: Not standard on all systems (often ignored).


---

24. Command: ls -z

Description: Ends each filename with a NUL instead of newline.
Output:

$ ls -z
file1.txt<NULL>file2.c<NULL>

Remarks: Safer for scripts when parsing filenames.
   




