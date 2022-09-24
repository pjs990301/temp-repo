1. pwd : Shows the current path in a hierarchical directory
<pre><code>$ PWD
/Users/pyojisung
</code></pre>

2. ls : List files and directories
<pre><code>$ ls
</code></pre>

3. Using arguments to control ls 
<pre><code>$ -l : Show detailed information (long format)
$ -lh : Same as above, but size in units
</code></pre>
<pre><code>Example 
$ ls  : List the files in the working directory
$ ls /bin : List the files in the /bin directory (or any other directory we care to specify)
$ ls -l : List the files in the working directory in long format
$ ls -l /etc / bin : List the files in the /bin directory and the /etc directory in long format
$ ls -la.. : List all files in the parent of the working directory in long format
</code></pre>


4. cd : Change directory
<pre><code>$ cd
</code></pre>

5. Using arguments to control cd 
<pre><code>$ / root
$ . current directory
$ .. upper-level directory
$ ~ home of current user
$ /[directory name] : absolute path
$ ./[directory name] : relative path
$ ../[directory name] : relative path
</code></pre>

5. cp : Copy files and directories
<pre><code>$ cp</code></pre>
   
   <pre><code>Example 
$ cp file1 file2 : Copies the contents of file1 into file2. if file2 does not exist, it is created; otherwise, file2 is silently overwritten withe the contents of file1.
$ cp -i file1 file2 : Like above however, since the "-i" (interactive) option is specified, if file2 exists, the user is prompted before it is overwritten with the contents of file1.
$ cp filel dirl : Copy the contents of file1 inside of directory dir1.
$ cp -R dirl dir2 : Copy the contents of the directory dir1. If directory dir2 does not exist, it is created. Otherwise, it creates a directory named dir1 within directory dir2.
</code></pre>
5. rm : Move files and directories **(permantely and irreversevely!!!)** or rename them 
<pre><code>$ rm</code></pre>

   <pre><code>Example 
$ rm file1 file2 : Delete file1 and file2.
$ rm -i file1 file2 : Like above however, since the "-i" (interactive) option is specified, the user is prompted before each file is deleted.
$ rm -r dir1 dir2 : Directories dir1 and dir2 are dleted along with all of their contents.
</code></pre>

6. mkdir : Make a new directory
<pre><code>$ mkdir
</code></pre>

7. using Wildcards to control cd 
<pre><code>$ * : All filenames
$ g* : All filenames that begin with the character "g"
$ b*.text : All filenames that the begin with the character "b" and end with the characters ".txt"
$ Data?? : Any filename that begins with the characters "Data" followed by exactly 3 more characters
</code></pre>

8. Help command : help
<pre><code>$ help cd 
</code></pre>

9. Help command : man
<pre><code>$ man cp
</code></pre>

10. Exiting terminal : exit
<pre><code>$ exit
</code></pre>


