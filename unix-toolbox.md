# Unix Toolbox and Resources

**Amazing Intro to Unix Blog Post -** [How Unix Works: Become a Better SWE](https://neilkakkar.com/unix.html)
  - Let’s start at the core - the philosophy behind Unix.
     - Write programs that do one thing and do it well.
     - Write programs to work together. (no extra output, don’t insist on interactive input)
     - Write programs to handle text streams, because that is a universal interface.
 - Unix also embraced the [“Worse is better”](https://blog.codinghorror.com/worse-is-better/) philosophy.
 - Everything is either Process or File
 - *Process* is a running instance of code. OS give resources to the process (like memory), then attaches some metadata (like who's the owner), and runs the code. Every process gets following 3 open files as resources: stdin, stdout, stderr
 - *File* - everything which is not a process. A file is stream of data.
 - *Shell* is the interface you use to interact with the operating system. It can be both, a command line interface (CLI), and graphical user interface (GUI)
 - chmod in verbose mode
    ```
    $ chmod u+rwx . # enable user for rwx
    $ chmod u-r .   # disable user for r
    $ chmod g+w .   # enable group for w
    $ chmod o+x .   # enable others for x
    ```
  - `>` redirects stdout to a file, and `>>` appends stdout to a file
  
**Conceptual intro to VIM** - [How not to be afraid of vim anymore](https://neilkakkar.com/How-not-to-be-afraid-of-Vim-anymore.html)
  - Vim modes: 1)normal, 2)insert
  - Command anatomy -> [action]{number}[motion] (e.g. d3w = **d**elete next **3** **w**ords)
  - Since actions on the entire line are very frequent, the developers of vim created a new shorthand for them — omitting the need to add a motion. Repeat the action to apply on the entire line. For example:
    - To delete the current line: dd
    - To copy the current line: yy



**Corey Schaffer's Linux/Mac Tutorials** ([youtube](https://www.youtube.com/watch?v=j6vKLJxAKfw&list=PL-osiE80TeTvGhHkpvfmKWOiIPF8UVy6c))
 - [Mac OS X Terminal: time-saving shortcuts](https://www.youtube.com/watch?v=TXzrk3b9sKM&list=PL-osiE80TeTvGhHkpvfmKWOiIPF8UVy6c&index=11))
    - hold option key and click on any point  - move cursor anywhere
    - ctrl + u   -> remove everything before the cursor
    - ctrl + k   -> remove everything after the cursor
    - write "cd" and grab-and-drag any folder on your desktop to terminal screen
    - run "!<text>"  -> run most recent command in history starting with $history
    - ctrl + r -> reverse search of commands
    - $clear or ctrl + l  ->  clear the screen (but not scroll-back)
    - cmd + k  -> clear the screen (and also the scroll-back)
 - [How to use the cURL command](https://www.youtube.com/watch?v=WxUVU0b95Oc&list=PL-osiE80TeTvGhHkpvfmKWOiIPF8UVy6c&index=5)
    - $ curl <URL>   -> will get back html script (as browser's are rendering)
    [useful when testing REST applications]
    - $ cur
    
jq Manual at https://stedolan.github.io/jq/manual/ (jq is a lightweight and flexible command-line JSON processor)
    
[Linux vs Unix: What's the difference](https://opensource.com/article/18/5/differences-between-linux-and-unix)

**Intro to unix tele typewriter** - [The TTY demystified](http://www.linusakesson.net/programming/tty/index.php)
