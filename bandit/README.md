# overthewire

Solutions for overthewire
all that is written in <code>commands</code> are to be written in terminal

<h1>Bandit</h1>

<h2>level 0</h2>
<p>tip: ssh username@website -p &ltport num&gt</p>
<details>
<summary>ans</summary>
<code>ssh bandit0@bandit.labs.overthewire.org -p 2220</code>

<p>the password is <code>bandit0</code></p>

<p>then, type <code>ls</code></p>
<p><code>cat readme</code></p>
<p><code>exit</code></p>
<p> pswd: NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL</p>
</details>

<h2>level 1</h2>
<details>
<summary>ans</summary>
<p><code>ssh bandit1@bandit.labs.overthewire.org -p 2220</code></p>
<p>the password is <code>NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL</code></p>
<p><code>ls</code></p>
<p><code>cat ./-</code></p>
<p><code>exit</code></p>
<p> pswd: rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi</p>
</details>

<h2>level 2</h2>
<details>
<summary>ans</summary>
<p><code>ssh bandit2@bandit.labs.overthewire.org -p 2220</code></p>
<p><code>rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi</code></p>
<p><code>ls</code></p>
<p><code>"spaces in this filename"</code></p>
<p><code>exit</code></p>
<p> pswd: aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG</p>
</details>

<h2>level 3</h2>
<details>
<summary>ans</summary>
<p><code>ssh bandit3@bandit.labs.overthewire.org -p 2220</code></p>
<p><code>aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG</code></p>
<p><code>ls</code></p>
<p><code>cd inhere</code></p>
<p><code>ls -a</code></p>
<p><code>cat ./.hidden</code>
<p><code>exit</code></p>
<p> pswd: 2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe</p>
</details>

<h2>level 4</h2>
<details>
<summary>ans</summary>
<p><code>ssh bandit4@bandit.labs.overthewire.org -p 2220</code></p>
<p><code>2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe</code></p>
<p><code>ls</code></p>
<p><code>cd inhere</code></p>
<p><code>ls -al</code></p>
<p>cat every file<br>here <code>cat ./-file07</code></p>
<p><code>exit</code></p>
<p> pswd: lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR</p>
</details>

<h2>level 5</h2>
<p>tip: enter <code>find --help</code> and try to write the parameters
<details>
<summary>ans</summary>
<p><code>ssh bandit5@bandit.labs.overthewire.org -p 2220</code></p>
<p><code>lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR</code></p>
<p><code>ls</code></p>
<p><code>cd inhere</code></p>
<p><code>find -size 1033c ! -executable</code></p>
<p>c means files in bytes<br><code>cat ./maybehere07/.file2</code></p>
<p><code>exit</code></p>
<p> pswd: P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU</p>
</details>

<h2>level 6</h2>
<details>
<summary>ans</summary>
<p><code>ssh bandit6@bandit.labs.overthewire.org -p 2220</code></p>
<p><code>P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU</code></p>
<p>here, we have to find in the server</p>
<p><code>find / -type f -user bandit7 -group bandit6 -size 33c</code></p>
<p>/ is the root directory</p>
<p><code>cat ./var/lib/dpkg/info/bandit7.password</code></p>
<p><code>exit</code></p>
<p> pswd: z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S</p>
</details>

<h2>level 7</h2>
<p>tip: enter <code>grep --help</code> and try to write the parameters
<details>
<summary>ans</summary>
<p><code>ssh bandit7@bandit.labs.overthewire.org -p 2220</code></p>
<p><code>z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S</code></p>
<p><code>ls</code></p>
<p><code>grep -i 'millionth' data.txt</code></p>
<p>-i means to ignore case</p>
<p><code>exit</code></p>
<p> pswd: TESKZC0XvTetK0S9xNwm25STk5iWrBvP</p>
</details>

<h2>level 8</h2>
<p>tip: you need to mess around with the commands given there
<details>
<summary>ans</summary>
<p><code>ssh bandit8@bandit.labs.overthewire.org -p 2220</code></p>
<p><code>TESKZC0XvTetK0S9xNwm25STk5iWrBvP</code></p>
<p><code>ls</code></p>
<p><code>sort data.txt | uniq -c | grep '1 '</code></p>
<p>sort sorts data in the file in alphanumeric order</p>
<p> | is called piping where each command is executed one after in other</p>
<p> uniq doesn't work properly unless they are sorted.</p>
<p> -c shows count of how many times it was repeated and displyes entries once</p>
<p> so we sort the data then through 'piping' we print repeated entries with their count and then find line with count 1 with grep</p>
<p><code>exit</code></p>
<p> pswd: EN632PlfYiZbn3PhVK3XOGSlNInNE00t</p>
</details>
