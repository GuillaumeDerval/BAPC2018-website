---
layout: default
title: System
menutitle: System
order: 4
menu: contest
---

<p>The information on this page is subject to change. Please check later for the
definitive information. The machines are PCs with an installation based on the
Jessie release of Debian GNU/Linux amd64. It is allowed to bring your own simple
keyboard. Programmable keyboards are not allowed. We provide a simple mouse and
it is not allowed to bring your own mouse.  This page lists the available
software. Documentation for mono will be available on the system through monodoc.
There will also be online documentation for C, C++, Java and Python 2/3 available
(but of course no internet access). The offline version of cppreference.com is
also available.</p>

<h4 id="compilation-options">Compilation Options</h4>

<p>All programs will run with a 1,5GB memory limit. Because of JVM overhead, a
little more than 1200MB of heap space is available to Java programs.</p>

<h5>C:</h5>

<div class="alert alert-secondary">
<code class="text-dark language-cmake">gcc -g -Wall -O2 -std=gnu99 -static -pipe -o $DEST <span class="s2">"$@"</span> -lm</code>
</div>

<h5>C++14:</h5>

<div class="alert alert-secondary">
<code class="text-dark language-cmake" data-lang="cmake">g++ -g -Wall -O2 -std=c++14 -static -pipe -o $DEST <span class="s2">"$@"</span></code>
</div>

<h5>Java compilation:</h5>

<div class="alert alert-secondary">
<code class="text-dark language-cmake" data-lang="cmake">javac -encoding UTF-8 -d . <span class="s2">"$@"</span></code>
</div>

<h5>Java runtime:</h5>
<div class="alert alert-secondary">
<code class="text-dark language-cmake" data-lang="cmake">java -Xrs -Xss512m -Xmx1272864k $MAINCLASS</code>
</div>

<h5>Mono compilation (companies only):</h5>

<div class="alert alert-secondary">
<code class="text-dark language-cmake" data-lang="cmake">mcs -o+ <span class="s2">"$@"</span></code>
</div>
<p>There will be aliases available on the system in the format of  
<strong><code class="text-danger">mygcc</code></strong>,
<strong><code class="text-danger">myg++</code></strong>, 
<strong><code class="text-danger">myg11</code></strong>,
<strong><code class="text-danger">myjavac</code></strong>,
<strong><code class="text-danger">myjava</code></strong> 
and
<strong><code class="text-danger">mcs</code></strong>.
</p>

<h4 id="compilersinterpreters">Compilers/interpreters</h4>

<p>To be announced.</p>

<!--
<p><strong>C, C++, C++14</strong></p>
<ul>
  <li>GCC 5.4.0 (Ubuntu 5.4.0-6ubuntu1~16.04.4)</li>
</ul>

<p><strong>Java</strong></p>
<ul>
  <li>Java SE Runtime 1.8.0_144</li>
  <li>Java SE Runtime Environment (build 1.8.0_144-b01)</li>
  <li>Java HotSpot(TM) 64-Bit Server VM (build 25.144-b01, mixed mode)</li>
</ul>

<p><strong>Python</strong></p>
<ul>
  <li>Python 2.7.12 (<a href="/contest/python2_modules.txt">Available modules</a>)</li>
  <li>Python 3.5.2 (<a href="/contest/python3_modules.txt">Available modules</a>)</li>
</ul>

<p><strong>C#</strong></p>
<ul>
  <li>Mono 4.2.1</li>
</ul>
-->
<h4 id="editors">Editors</h4>

<p>To be announced.</p>
<!--
<ul>
  <li>Emacs 24.5.1</li>
  <li>Vim 7.4</li>
  <li>Eclipse 3.8 with CDT 8.6</li>
  <li>IntelliJ IDEA CE 2017 2.3</li>
  <li>Netbeans 8.1</li>
  <li>Nano 2.5.3</li>
  <li>Kate 16.04.3</li>
  <li>Gedit 3.18.3</li>
  <li>Geany 1.27</li>
  <li>KWrite 16.04.3</li>
  <li>KDevelop 5.1.1</li>
  <li>MonoDevelop 5.10</li>
  <li>CodeBlocks 13.12</li>
  <li>joe 4.1</li>
  <li>Sublime Text 3</li>
</ul>
-->