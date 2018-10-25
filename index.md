---
layout: default
menutitle: Home
title: BAPC 2018 - Saturday 27/10
order: 0
menu: main
---

<div class="container topinfo">
    <div class="row">
        <div class="col">
            <a href="http://d379jbr12qwxxc.cloudfront.net/public/"><b>Live scoreboard (on-site contest)</b></a>
        </div>
        <div class="col">
            <a href="http://d3lg6vvxjgtsmy.cloudfront.net/"><b>Contestant live streaming</b></a>
        </div>
        <div class="col">
            <a href="https://www.youtube.com/watch?v=QeMVF4Yok7k">Award ceremony live streaming</a>
        </div>
    </div>
    <div class="row">
        <div class="col">
            <a href="http://bapc2018-open.eu-central-1.elasticbeanstalk.com">Online public contest</a>
        </div>
        <div class="col">
            <a href="http://bapc2018-open.eu-central-1.elasticbeanstalk.com/register">Register for the online contest here</a>
        </div>
    </div>
    <div class="row">
        <div class="col"><b>Watch the presentation of the solutions and the award ceremony live at 18h30!</b>
        <br/>
        <iframe width="560" height="315" src="https://www.youtube.com/embed/QeMVF4Yok7k" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
        </div>
    </div>
</div>



### About the BAPC 

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
