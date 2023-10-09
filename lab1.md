# Lab Report 1

**Command "cd" With No Arguments**
```
[user@sahara ~]$ cd
[user@sahara ~]$ 
```
The working directory was still the root (/home) after running the command.\
It prompts the user as if we changed the directory to the root.\
I got this output because there was no argument, so cd had no directory to redirect to.\
This output is not an error.

---

**Command "cd" With Path to Directory as Argument**
```
[user@sahara ~]$ cd lecture1/messages
[user@sahara ~/lecture1/messages]$ 
```
The working directory was "~/lecture1/messages" after running the command.\
I got this result because the path was an absolute path to a working directory.\
This output is not an error.

---

**Command "cd" With Path to File Argument**
```
[user@sahara ~]$ cd lecture1/Hello.class
bash: cd: lecture1/Hello.class: Not a directory
```
The working directory was still the root, /home.\
I got this output because the file that I chose was not a directory, so it was an invalid path to put as an argument.\
This output is not an error.

---


**Command "ls" With No Arguments**
```
[user@sahara ~]$ ls
lecture1
[user@sahara ~]$ 
```
The working directory is still the root.\
I got this output because the root is considered a directory and it displayed all direct paths (lecture1).\
This output is not an error.

---

**Command "ls" With Path to Directory as Argument**
```
[user@sahara ~]$ ls lecture1
Hello.class  Hello.java  messages  README
[user@sahara ~]$ 
```
The working directory is still the root.\
I got this output because the path was valid and was to a directory.\
The contents that were output were files/directories directly in lecture1.\
This output is not an error.

---

**Command "ls" With Path to File Argument**
```
[user@sahara ~]$ ls lecture1/README
lecture1/README
[user@sahara ~]$ 
```
The working directory is the root.\
I got this output because the path was to a file, which does not contain other folders and files.\
This output is not an error.

---

**Command "cat" With No Arguments**
```
[user@sahara ~]$ cat






```
The working directory is the root.\
This was the output because there was no path for the command to use.\
This is an error because the command requires a path for it to work.

---

**Command "cat" With Path to Directory as Argument**
```
[user@sahara ~]$ cat lecture1/messages
cat: lecture1/messages: Is a directory
[user@sahara ~]$ 
```
The working directory is still the root.\
This was the output because a directory does not have contents in it, just files and other directories.\
This output is not an error.

---

**Command "cat" With Path to File Argument**
```
[user@sahara ~]$ cat lecture1/Hello.java
import java.io.IOException;
import java.nio.charset.StandardCharsets;
import java.nio.file.Files;
import java.nio.file.Path;

public class Hello {
  public static void main(String[] args) throws IOException {
    String content = Files.readString(Path.of(args[0]), StandardCharsets.UTF_8);    
    System.out.println(content);
  }
}[user@sahara ~]$ 
```
The working directory was still the root after running the command.\
This was the output because the command printed the entire contents of the file Hello.java.\
This output is not an error.
