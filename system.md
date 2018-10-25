---
layout: default
title: System
menutitle: System
order: 4
menu: contest
---

<p><b>The information on this page is subject to change</b>. Please check later for the
definitive information. The machines are PCs with an installation based on ArchLinux amd64. 

It is allowed to bring your own simple keyboard. Programmable keyboards are not allowed. 
We provide a simple mouse and it is not allowed to bring your own mouse.  This page lists the available
software. The documentation for C, C++, Java, C# (Mono) and Python 2/3 will be available on 
[Zeal](https://zealdocs.org/).</p>

<h4 id="compilation-options">Compilation Options</h4>

<p>All programs will run with a 1,5GB memory limit. Because of JVM overhead, a
little more than 1200MB of heap space is available to Java programs.</p>

<h5>C:</h5>

<div class="alert alert-secondary">
<code class="text-dark language-bash">gcc -x c -Wall -O2 -std=gnu99 -static -pipe -o $DEST <span class="s2">"$@"</span> -lm</code><br/>
(Flag <code class="text-dark language-bash">-g</code>, that enables debugging, is present in the <code class="text-danger">mygcc</code> command but not on the judge)
</div>

<h5>C++14:</h5>

<div class="alert alert-secondary">
<code class="text-dark language-bash" data-lang="cmake">g++ -x c++ -Wall -O2 -std=c++14 -static -pipe -o $DEST <span class="s2">"$@"</span></code><br/>
</div>
(Flag <code class="text-dark language-bash">-g</code>, that enables debugging, is present in the <code class="text-danger">myg++</code> command but not on the judge)

<h5>Java compilation:</h5>

<div class="alert alert-secondary">
<code class="text-dark language-bash" data-lang="cmake">javac -encoding UTF-8 -d . <span class="s2">"$@"</span></code>
</div>

<h5>Java runtime:</h5>
<div class="alert alert-secondary">
<code class="text-dark language-bash" data-lang="cmake">java -Xrs -XX:+UseSerialGC -Xss65536k -Xms1441792k -Xmx1441792k $MAINCLASS</code>
</div>

<h5>C# using Mono (companies only):</h5>

<div class="alert alert-secondary">
<code class="text-dark language-bash" data-lang="cmake">mcs -o+ <span class="s2">"$@"</span></code>
</div>

<h5>Python 2/3:</h5>

<div class="alert alert-secondary">
<code class="text-dark language-bash" data-lang="cmake">pypy <span class="s2">"$@"</span></code><br/>
<code class="text-dark language-bash" data-lang="cmake">pypy3 <span class="s2">"$@"</span></code><br/>
</div>
<code class="text-dark language-bash">python</code> and <code class="text-dark language-bash">python3</code> will 
respectively redirect to <code class="text-dark language-bash">pypy</code> and 
<code class="text-dark language-bash">pypy3</code>.

<h5>Aliases</h5>

<p>There will be aliases available on the system in the format of  
<strong><code class="text-danger">mygcc</code></strong>,
<strong><code class="text-danger">myg++</code></strong>, 
<strong><code class="text-danger">myjavac</code></strong>,
<strong><code class="text-danger">myjava</code></strong>,
<strong><code class="text-danger">mypython2</code></strong>,
<strong><code class="text-danger">mypython3</code></strong>,
and
<strong><code class="text-danger">mymcs</code></strong>.
</p>

<h4 id="compilersinterpreters">Compilers/interpreters</h4>

<p><strong>C, C++</strong></p>
<ul>
  <li>GCC/G++ 8.2.1</li>
</ul>

<p><strong>Java</strong></p>
<ul>
  <li>Java 10 - OpenJDK 10.0.2</li>
</ul>

<p><strong>Python</strong></p>
<ul>
  <li>Python 2.7.13 - using Pypy2.7 6.0.0</li>
  <li>Python 3.5.3 - using Pypy3.5 6.0.0</li>
</ul>

<p><strong>C#</strong></p>
<ul>
  <li>Mono 5.14.0</li>
</ul>

<h4 id="editors">Editors</h4>
<ul>
  <li>Emacs 26.1</li>
  <li>Vim 8.1.470</li>
  <li>Eclipse 4.9-1</li>
  <li>IntelliJ IDEA CE 2018.2.5</li>
  <li>Netbeans 9.0</li>
  <li>Nano 3.1</li>
  <li>Kate 18.08.0</li>
  <li>Gedit 3.30.2</li>
  <li>Geany 1.33</li>
  <li>KWrite 18.08.2</li>
  <li>KDevelop 5.2.4</li>
  <li>MonoDevelop 7.8.0</li>
  <li>CodeBlocks 17.12</li>
  <li>Sublime Text 2.0.2</li>
  <li>Pycharm CE 2018.2.4</li>
</ul>

<h4>Other tools</h4>
<ul>
    <li>Make 4.2.1</li>
    <li>GDB 8.2</li>
    <li>Valgrind 3.14.0</li>
    <li>Git 2.19.1</li>
    <li>Screen 4.06.02</li>
    <li>Tmux 2.8</li>
    <li>Galculator 2.1.4</li>
    <li>Evince 3.30.2</li>
</ul>