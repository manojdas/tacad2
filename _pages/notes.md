---
layout: page
permalink: /notes/
title: notes
description: Lecture notes from classes I have taken and notes from seminars I have attended.
years: [2021, 2019, 2018, 2017, 2016, 2015, 2013]
nav: true
nav_order: 1
series: [Combinatorics, Reading Group]
---


{:.no_toc}

* Will be replaced with the ToC, excluding the "Contents" header
{:toc}


### Lecture Notes
<!-- <hr> -->

### Combinatorics Seminar
    {% assign notes = site.seminar_notes | where: 'series', 'Combinatorics' | sort: 'date' %}

<ul class='sd-seminar-notes'>
    {% for note in notes %}
        {% include talks.html talk=note %}
    {% endfor%}
</ul>


### Reading Group Seminar
    {% assign notes = site.seminar_notes | where: 'series', 'Reading Group' | sort: 'date' %}

<ul class='sd-seminar-notes'>
    {% for note in notes %}
        {% include talks.html talk=note %}
    {% endfor%}
</ul>



