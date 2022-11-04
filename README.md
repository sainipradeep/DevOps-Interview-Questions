## Script

<ol>
<li>
Using the command line, make an HTTP GET request to the following endpoint and save the output to a local file called "users.json":<br>
http://localhost:5000/users
</li>
<li>
Using Python 3, NodeJs, or Java 8, write a program to convert "users.json" into "users.csv". Only built in libraries are permitted.
</li>

<li>
Normalize Path Given a string s containing an absolute Unix-based directory path write a program hat normalizes this path using the following rules.
</li>
<ul>
<li>
 Remove . from the path, which means stay in the same directory: /a/./b becomes /a/b
</li>
<li>
 Remove .. from the path, which means go to the parent directory: /a/../b becomes /b
</li>
<li>
 Remove consecutive / characters from the path: /a////b becomes /a/b
</li>
<li>
 Remove trailing / characters from the path: /a/b/ becomes /a/b
</li>
<li>
 Paths cannot go beyond the root directory: /../a becomes /a
</li>
<li>
 All other path characters are valid: ..., null, spaces.
</li>
<li>
 The method must return the normalized path a string.
</li>
</ul>
<pre>
 Input: "/usr/local/./../bin/."
 Output: "/usr/bin"
<br>
 Input: "/home/../.."
 Output: "/"
<br>
 Input: "/etc/system/../../home/user"
 Output: "/home/user"
<br>
## Solutions
<a href="./coding/nodejs/README.md## Normalization directory path">
NodeJS
</a>
</pre>
</ol>

## Operating System

<ol>
<li>
You run the command du over a filesystem. The file system is full, but if you look into it you see no files. What's happening? how can you solve it?
</li>
<li>
You are logged in a shell, you try to run ps command and it fails with 'cannot fork' error while if you run echo it works. What's happening? how can you fix it?
</li>
</ol>
