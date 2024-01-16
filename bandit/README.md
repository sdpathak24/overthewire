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
