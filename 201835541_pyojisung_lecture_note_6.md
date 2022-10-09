# Lab6

### installing Git
1. Linux / Mac / Windows (check pre-installed version)
<pre><code>$ git --version
git version 2.25.1
</code></pre>
2. Linux (install on a Debian-based distribution)
<pre><code>$ sudo apt install git-all 
</code></pre>
3. Mac   
[https://git-scm.com/downlad/mac](201835541_pyojisung_lecture_note_5.md)
4. Windows - Run "Git Bash"   
[https://git-scm.com/downlad/win](201835541_pyojisung_lecture_note_5.md)

### Git config : First-time setup
#### Git configurations are stored in three levels :
1. System level : -- system option. Affects all uses and repositories on the system (administrative)   
**file : etc/gitconfig**
2. Global (user) level : --global option. Affects all repositories of a current user   
**file : ~/.config/git/config**
3. Local level : --local option. Specific to the current repository   
**file : .git/gitconfig**
4. Each level overrides values in the previous level system -> global -> local
   <pre><code>$ git config --list
   $ git config --list --show-origin
   </code></pre>

<pre><code>$ git config --global user.name "Jisung Pyo"
$ git config --global user.email your-email p990301@gachon.ac.kr
$ git config --global init.defaultBranch main
$ git config --list
$ git config --list --show-origin
$ git config user.name
Jisung pyo
</code></pre>

### Initializing a Repository in an Existing Directory
<pre><code>$ git init
Initialized empty Git repository in /home/OSS/.git/
</code></pre>

### Checking Repository Status
<pre><code>$ git status

On branch master
Your branch is up to date with 'origin/master'.

nothing to commit, working tree clean
</code></pre>

### Adding a new file to be staged (tracked)
<pre><code>$ git add [file_name]
$ git add README.md
</code></pre>

### Adding all files to be staged (tracked)
<pre><code>$ git add.
</code></pre>

### Unstaging a file
<pre><code>$ git rm -- cached [file_name]
$ git rm -- cached history_command.txt
rm 'history_command.txt'
</code></pre>

### Ignoring a file
<pre><code>$ nano .gitignore
</code></pre>

### Commit
<pre><code>$ git commit -m "commit message"
</code></pre>

### change branch name
<pre><code>$ git branch
* master

$ git branch -m master main
$ git branch
* main

$ git status
On branch main
nothing to commit, working tree clean
</code></pre>