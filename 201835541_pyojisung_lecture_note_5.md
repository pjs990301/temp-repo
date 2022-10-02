#Lab5

### I/O Redirection : Standard Output
1. Redirect output using ">"
<pre><code>$ ls -lh
$ ls -lh > file_list.txt
</code></pre>
2. Command "cat" displays the content of a text file.
<pre><code>$ cat file_list.txt
</code></pre>
3. Using ">>" app appends output to an extising file (if it already exitsts),<br>or create and write to a new file iif it doesn't exist
<pre><code>$ ls -lh
$ ls -lh >> file_list.txt
</code></pre>

### I/O Redirection : Standard Input
1. Standard input is from keyboard.
2. Redirect input from a file using "<".
3. Mix "<" and ">" together in a single line
<pre><code>$ cat word.txt
$ sort < words. txt > sorted_words.txt
$ cat sorted_words.txt
</code></pre>

### Pipelines "l"
1. Pipeline feeds output of previous command to input of next command.
2. command1 | command2 | command3 | ...
<pre><code>$ ls -lh | less
</code></pre>
3. press "q" key to exit the screen.

### Expansion
1. Special characters expand its meaning meaning when given to shell commands.
<pre><code>$ echo print out the text
print out the txt

$ echo *
READM.md word.txt

$ echo ~
/home/pyojisung

$ echo ~ pyojisung
/home/pyojisung
</code></pre>

### Tip : Backslash
1. Backslash can be used to ignore line change in command ("Enter"), to enter a long command in multiple lines.
<pre><code>$ ls -l \
> --reverse \
> --human-readbel
</code></pre>

### Permissions
1. Linux is a multi-user system.
2. Files and directories have a permission assigned differently to owner / group / others.
<pre><code>$ ls -ㅣ /bin/bash
--rwxr-xr-x 1 root root 
</code></pre>

### Changing Permissions
1. "Chmod" changes permissions
<pre><code>$ chmod 600 some_file
6 = 110 = rw- for owner
0 = 000 = --- for group
0 = 000 = --- for others
</code></pre>

### Superuser
1. A superuser has all system administration authority.
2. Some commands need superuser's privilleges.
3. Put "sudo" before the command if you are a superuser.
<pre><code>$ sudo some_command
Password for me:
</code></pre>
<pre><code>$ sudo -i
Password for me:
</code></pre>
4. type "exit" to get out of a superuser session.
