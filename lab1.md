# Lab Report 1

**Command "cd" With No Arguments**\
```
[user@sahara ~]$ cd
[user@sahara ~]$ 
```
The working directory was still the root (~) after running the command.\
It prompts the user as if we changed the directory to the root.\
I got this output because there was no argument, so cd had no directory to redirect to.\
This was not an error, as 


**Command "cd" With Path to Directory as Argument**\
```
[user@sahara ~]$ cd lecture1/messages
[user@sahara ~/lecture1/messages]$ 
```
The working directory was ~/lecture1/messages after running the command.\
I got this result because the path was an absolute path to a working directory.\
This is not an error, since if I were to just put the relative path, the terminal would find difficulty \
in finding the "messages" directory.\


**Command "cd" With Path to File Argument**\
```
[user@sahara ~]$ cd lecture1/Hello.class
bash: cd: lecture1/Hello.class: Not a directory
```
The working directory was still the root, ~.\
I got this output because the file that I chose was not a directory, so it was an invalid path to put as an argument.\
This is not an error because the argument of the path required is supposed to be a directory, not a file.\



**Command "ls" With No Arguments**\
```
[user@sahara ~]$ ls
lecture1
[user@sahara ~]$ 
```

**Command "ls" With Path to Directory as Argument**\
```
[user@sahara ~]$ ls lecture1
Hello.class  Hello.java  messages  README
[user@sahara ~]$ 
```

**Command "ls" With Path to File Argument**\
```
[user@sahara ~]$ ls lecture1/README
lecture1/README
[user@sahara ~]$ 
```

**Command "cat" With No Arguments**\
```
[user@sahara ~]$ cat






```
The 

**Command "cat" With Path to Directory as Argument**\
```
[user@sahara ~]$ cat lecture1/messages
cat: lecture1/messages: Is a directory
[user@sahara ~]$ 
```
The 

**Command "cat" With Path to File Argument**\
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
