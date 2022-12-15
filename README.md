# Linux
## LINUX command line

1. change directories `cd`
2. tree structure `tree`
3. list their contents `ls` (`-l` for the long format )
4. rename or move files  `mv`
5. print working directory `pwd`
6. make directory  `mkdir`
7. concentrate files or read `cat output.txt` (`cat -A output.txt` to display text, `-nl` for number line )
8. write (overwrite) in text file `cat > output.txt`(only append ~~overwrite~~ in text file `cat >> output.txt`), finish with *Ctrl-d*
9. append or combine text file `cat file1.txt file2.txt > combinedfile.txt`
10. print something `echo <something>`
11. move to dir1 `mv <filename> <to_directory>`
12. copy with a different name `cp output.txt renamed_output.txt`
13. remove `rmdir <folder>`
14. delete the whole directory and anything within it `rm -r folder_6` (recursively `-r`)
15. word count in docs `wc -l combined.txt` (line count `-l`)
16. brief description `file <filename>`
17. clear screen `clear`
18. command history `history`
19. user id `id`
20. change the user password `passwd`
21. display tasks `top`
22. shutdown or reboot `shutdown`
23. finding the package in the repository `apt-get update`, `apt-cache search <search_string>`
24. install packages `apt-get update`, `apt-get install <package_name>`
25. install package from package file `dpkg -i <package file>`
26. remove package `apt-get remove <package_name>`
27. update packages `apt-get update`; `apt-get upgrade`
28. list of installed packages `dpkg -l`
29. package status `dpkg -s <package_name>`
30. package file identification `dpkg -S <file_name>`
31. file download from website `wget <url>`
32. file search `locate <filename>`
