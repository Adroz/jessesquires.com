---
layout: standalone
title: Curriculum Vitae
---

<h5 class="text-muted"><small><i>Updated: 28 March 2020</i></small></h5>

**I'm currently available for iOS freelance and contracting.**
If you're interested in working together, please **[get in touch](/contact)**.

{% assign resume = site.data.resume %}

<!-- WORK -->

{% include resume_section.html resume_section=resume.work %}

<!-- PROJECTS -->

<h3>Projects & Open Source</h3>

<p>See <a href="/projects">projects</a>, my <a href="{{ site.social_links.github }}">GitHub profile</a>, and <a href="https://www.hexedbits.com">Hexed Bits</a>.</p>

<h3>Conference Talks</h3>

<p>See <a href="/speaking">speaking</a>.</p>

<!-- SKILLS -->

<h3>{{ resume.skills.title }}</h3>

<ul class="list-inline">
{% for entry in resume.skills.entries %}
<li class="list-inline-item">{{ entry }}</li>
<li class="list-inline-item">{% if resume.skills.entries.last != entry %}&bull;{% endif %}</li>
{% endfor %}
</ul>

<!-- VOLUNTEERING -->

{% include resume_section.html resume_section=resume.volunteering %}

<!-- EDUCATION -->

{% include resume_section.html resume_section=resume.education %}

<!-- RESEARCH -->

{% include resume_section.html resume_section=resume.research %}

<!-- PUBLICATIONS -->

{% include resume_section.html resume_section=resume.publications %}
