---
layout: page
permalink: /notes/
title: notes
description: Lecture notes from classes I have taken and notes from seminars I have attended.
years: [2021, 2019, 2018, 2017, 2016, 2015, 2013]
nav: true
nav_order: 1
---


{:.no_toc}

* Will be replaced with the ToC, excluding the "Contents" header
{:toc}


## Lecture Notes
<!-- <hr> -->





## Combinatorics Seminar
<!-- <hr> -->
{% assign notes = site.seminar_notes | where: 'series', 'combinatorics' | sort: 'date' %}

<ul class='sd-seminar-notes'>
{% for note in notes %}
    <li>
        <div class="title">
            {{ note.title }}
        </div>
        <div class="author">
            {{ note.presenters }}
        </div>
        <p class="post-meta">
            {{ note.date | date: '%B %-d, %Y' }}
        </p>
    </li>
{% endfor%}
</ul>



## Reading Group Seminar
<!-- <hr> -->

