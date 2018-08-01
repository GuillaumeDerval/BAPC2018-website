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
software. Documentation for mono will be available on the system through monodoc.
There will also be online documentation for C, C++, Java and Python 2/3 available
(but of course no internet access). The offline version of cppreference.com is
also available.</p>

<h4 id="compilation-options">Compilation Options</h4>

<p>All programs will run with a 1,5GB memory limit. Because of JVM overhead, a
little more than 1200MB of heap space is available to Java programs.</p>

<h5>C:</h5>

<div class="alert alert-secondary">
<code class="text-dark language-cmake">gcc -x c -Wall -O2 -std=gnu99 -static -pipe -o $DEST <span class="s2">"$@"</span> -lm</code><br/>
(Flag <code class="text-dark language-cmake">-g</code>, that enables debugging, is present in the <code class="text-danger">mygcc</code> command but not on the judge)
</div>

<h5>C++14:</h5>

<div class="alert alert-secondary">
<code class="text-dark language-cmake" data-lang="cmake">g++ -x c++ -Wall -O2 -std=c++14 -static -pipe -o $DEST <span class="s2">"$@"</span></code><br/>
(Flag <code class="text-dark language-cmake">-g</code>, that enables debugging, is present in the <code class="text-danger">myg++</code> command but not on the judge)
</div>

<h5>Java compilation:</h5>

<div class="alert alert-secondary">
<code class="text-dark language-cmake" data-lang="cmake">javac -encoding UTF-8 -d . <span class="s2">"$@"</span></code>
</div>

<h5>Java runtime:</h5>
<div class="alert alert-secondary">
<code class="text-dark language-cmake" data-lang="cmake">java -Xrs -XX:+UseSerialGC -Xss65536k -Xms1441792k -Xmx1441792k $MAINCLASS</code>
</div>

<h5>C# using Mono (companies only):</h5>

<div class="alert alert-secondary">
<code class="text-dark language-cmake" data-lang="cmake">mcs -o+ <span class="s2">"$@"</span></code>
</div>

<h5>Python 2/3:</h5>

<div class="alert alert-secondary">
<code class="text-dark language-cmake" data-lang="cmake">python2 <span class="s2">"$@"</span></code><br/>
<code class="text-dark language-cmake" data-lang="cmake">python3 <span class="s2">"$@"</span></code>
</div>

<p>There will be aliases available on the system in the format of  
<strong><code class="text-danger">mygcc</code></strong>,
<strong><code class="text-danger">myg++</code></strong>, 
<strong><code class="text-danger">myg11</code></strong>,
<strong><code class="text-danger">myjavac</code></strong>,
<strong><code class="text-danger">myjava</code></strong>
and
<strong><code class="text-danger">mymcs</code></strong>.
</p>

<h4 id="compilersinterpreters">Compilers/interpreters</h4>

<p>To be announced.</p>


<p><strong>C, C++, C++14</strong></p>
<ul>
  <li>GCC/G++ 8.1</li>
</ul>

<p><strong>Java</strong></p>
<ul>
  <li>Java SE Runtime 1.8.0_171</li>
  <li>Java SE Runtime Environment (build 1.8.0_144-b01)</li>
  <li>Java HotSpot(TM) 64-Bit Server VM (build 25.144-b01, mixed mode)</li>
</ul>

<p><strong>Python</strong></p>
<ul>
  <li>Python 2.7.15</li>
  <li>Python 3.6.5</li>
</ul>

<p><strong>C#</strong></p>
<ul>
  <li>Mono 5.12.0</li>
</ul>

<h4 id="editors">Editors</h4>
<ul>
  <li>Emacs 26.1</li>
  <li>Vim 8.1</li>
  <li>Eclipse (version TBA)</li>
  <li>IntelliJ IDEA CE (version TBA)</li>
  <li>Netbeans (version TBA)</li>
  <li>Nano 2.9.8</li>
  <li>Kate 18.04.0</li>
  <li>Gedit 3.28.1</li>
  <li>Geany 1.33</li>
  <li>KWrite 18.04.2</li>
  <li>KDevelop 5.2.3</li>
  <li>MonoDevelop (version TBA)</li>
  <li>CodeBlocks (version TBA)</li>
  <li>Sublime Text 3</li>
  <li>Pycharm CE (version TBA)</li>
</ul>

<h4>Other tools</h4>
<ul>
    <li>Make 4.2.1</li>
    <li>GDB 8.1</li>
    <li>Valgrind 3.13.0</li>
    <li>Git 2.17.1</li>
    <li>Screen 4.06.02</li>
    <li>Tmux 2.7</li>
    <li>Galculator 2.1.4</li>
</ul>