---
layout: default
menutitle: Home
title: About the BAPC
order: 0
menu: main
---

**The registration deadline for all teams is the 2nd of October 2018 at noon.**

The preliminary results are now <a href='https://2018.bapc.eu/preliminaries.html'>available</a>!

The Benelux Algorithm Programming Contest (BAPC) is a contest in which about 50 teams from leading universities in Luxemburg, 
Belgium and the Netherlands are served a series of algorithmic problems/puzzles. The goal of each team is to solve as many 
puzzles as possible within the set time limit. Solutions need to be programmed out on a computer and can be submitted to a 
semi-automated judging system, after which the solution is checked. The teams that have solved the most puzzles at the end 
of the contest qualify for the Northwestern European Regional Contest (NWERC). In this regional competition the teams can 
qualify themselves for a ticket to the International Collegiate Programming Contest (ICPC), also known as the World Finals.

The BAPC {{site.year}} will take place on <b>{{site.day}}</b> at Louvain-la-Neuve, Belgium and is co-organised by <a href='{{hostlink}}' target="_blank">{{site.hostname}}</a>
and <a href='https://web.umons.ac.be/en/' target="_blank">UMONS</a>.

#### Previous contests

<ul id="previousContests">
    {% assign previous = site.year | minus : 1 %}
    {% for i in (2010..previous) %}
        <li><a href="http://{{i}}.bapc.eu/" target="_blank">BAPC {{i}}</a></li>
    {% endfor %}
</ul>
