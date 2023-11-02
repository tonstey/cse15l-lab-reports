
# Part 1 - Bugs

# Part 2 - Researching Commands

1. -e Command Line Option 

**Command** 
```
$ less -e find-results.txt
``` 
**Output**
```
technical/911report
technical/911report/chapter-1.txt
technical/911report/chapter-10.txt
technical/911report/chapter-11.txt
technical/911report/chapter-12.txt
technical/911report/chapter-13.1.txt
technical/911report/chapter-13.2.txt
technical/911report/chapter-13.3.txt
technical/911report/chapter-13.4.txt
technical/911report/chapter-13.5.txt
technical/911report/chapter-2.txt
technical/911report/chapter-3.txt
technical/911report/chapter-5.txt
technical/911report/chapter-6.txt
technical/911report/chapter-7.txt
technical/911report/chapter-8.txt
technical/911report/chapter-9.txt
technical/911report/preface.txt
find-results.txt (END)
```
Using the -e command line on a file allows us to run the less command normally, but automatically exits once the end of the file is read by simply pressing another button rather than specifically pressing q to quit. 

**Command** 
```
$ less -E technical/911report
```
**Output**
```
technical/911report is a directory
```
Using the -e command line on a directory is the same as using just the `less` command. Since the argument is not a file, it just says that the path is a directory. \
\
Source: https://phoenixnap.com/kb/less-command-in-linux <br>
<br>

2. -N Command Line Option

**Command** 
```
$less -N find-results.txt
```

**Output** 
```
      1 technical/911report
      2 technical/911report/chapter-1.txt
      3 technical/911report/chapter-10.txt
      4 technical/911report/chapter-11.txt
      5 technical/911report/chapter-12.txt
      6 technical/911report/chapter-13.1.txt
      7 technical/911report/chapter-13.2.txt
      8 technical/911report/chapter-13.3.txt
      9 technical/911report/chapter-13.4.txt
     10 technical/911report/chapter-13.5.txt
     11 technical/911report/chapter-2.txt
     12 technical/911report/chapter-3.txt
     13 technical/911report/chapter-5.txt
     14 technical/911report/chapter-6.txt
     15 technical/911report/chapter-7.txt
     16 technical/911report/chapter-8.txt
     17 technical/911report/chapter-9.txt
     18 technical/911report/preface.txt
find-results.txt (END)
```
Using the -N command line on a file allows us to run the less command normally, but automatically exits once the end of the file is read by simply pressing another button rather than specifically pressing q to quit.   

**Command** 
```
$ less -N technical/911report
```
**Output**
```
technical/911report is a directory
```
Using the -e command line on a directory is the same as using just the `less` command. Since the argument is not a file, it just says that the path is a directory. \
\
Source: https://phoenixnap.com/kb/less-command-in-linux 



3. f
4. f


