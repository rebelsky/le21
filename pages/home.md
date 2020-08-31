---
title: Liberal Education in the 21st Century
permalink: /home/
---
# Liberal Education in the 21st Century

**_This site is under development!_**

<dl class="dl-horizontal">
  <dt>Instructor</dt>
  <dd>
    <p><a href="{{ site.instructor_homepage }}">{{ site.instructor }}</a>
      [<a href="mailto:{{ site.instructor_email }}">{{ site.instructor_email | remove: "@grinnell.edu" }}</a>]</p>
  </dd>

  <dt>Meeting Times</dt>
  <dd>
    <ul class="list-unstyled">
      {% for item in site.meeting_times %}
        <li>{{ item | markdownify | remove: "<p>" | remove: "</p>" }}</li>
      {% endfor %}
    </ul>
  </dd>

  <dt>Office Hours</dt>
  <dd>
    <ul class="list-unstyled">
      {% for item in site.office_hours %}
        <li>{{ item | markdownify | remove: "<p>" | remove: "</p>" }}</li>
      {% endfor %}
    </ul>
  </dd>

  <dt>Individual Meetings</dt>
  <dd>
    <p><em>As scheduled on Wednesday afternoons</em></p>
  </dd>

  <dt>Writing mentors</dt>
  <dd>
    <ul class="list-unstyled">
    <li>Delaney Gaughan [<a href="mailto:gaughand@grinnell.edu">gaughand</a>]</li>
    <li>Helen St. John [<a href="mailto:stjohnhe@grinnell.edu">stjohnhe</a>]</li>
    </ul>
  </dd>

  {% if site.partners %}
  <dt>Partners</dt>
  <dd>
      <ul class="list-unstyled">
        {% for partner in site.partners %}
          <li>
            {{ partner.name }}
            [<a href="mailto:{{ partner.email }}">{{ partner.email | remove: "@grinnell.edu" }}</a>],
            {{ partner.role }} 
          </li>
        {% endfor %}
      </ul>
  </dd>
  {% endif %}

  {% if site.review_sessions %}
    <dt>Review Sessions</dt>
    <dd>
      <ul class="list-unstyled">
        {% for session in site.review_sessions %}
          <li>{{ session }}</li>
        {% endfor %}
      </ul>
    </dd>
  {% endif %}
  
  {% if site.textbook %}
    <dt>Textbook</dt>
    <dd>
      {{ site.textbook | markdownify | remove: "<p>" | remove: "</p>" }}
    </dd>
  {% endif %}
  
  {% if site.mentors %}
    <dt>Class Mentors</dt>
    <dd>
      <ul class="list-unstyled">
        {% for mentor in site.mentors %}
          <li>{{ mentor }}</li>
        {% endfor %}
      </ul>
    </dd>
  {% endif %}
  
  {% if site.mentor_sessions %}
    <dt>Mentor Sessions</dt>
    <dd>
      <ul class="list-unstyled">
        {% for session in site.mentor_sessions %}
          <li>{{ session | markdownify | remove: "<p>" | remove: "</p>" }}</li>
        {% endfor %}
      </ul>
    </dd>
  {% endif %}
  
  {% if site.tutors %}
    <dt>CS Tutors</dt>
    <dd>
      <ul class="list-unstyled">
        {% for tutor in site.tutors %}
          <li>{{ tutor }}</li>
        {% endfor %}
      </ul>
    </dd>
  {% endif %}
</dl>

## About this course
Welcome to _The Open Curriculum, Tutorial, and Liberal Education in the 21st Century_, a self-reflective section of Grinnell's Tutorial.  In this course, we will explore approaches to the liberal arts and to liberal education, considering how liberal education might and should change for the twenty-first century and reflecting on Grinnell's particular approaches to liberal education.

This is the first (and, I hope, only) offering of Tutorial within Grinnell's
seven-week term structure.   Because Tutorial traditionally meets for two
110-minute sessions per week over fourteen weeks, this Tutorial meets for
four 110-minute sessions per week over the seven-week term.  In particular.
Tutorial meets Monday, Tuesday, Thursday and Friday from 
3:00-4:50 p.m. CDT.

You can learn more about the course in [the syllabus](../syllabus/) and 
[the schedule](../schedule/).

{% if site.extra_homepage_text %}
{{ site.extra_homepage_text | markdownify }}
{% endif %}
