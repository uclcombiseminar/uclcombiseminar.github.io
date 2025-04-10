---
title: UCL Combinatorics Seminar
---

The University College London (UCL) Combinatorics Seminar is held every Monday at 4&ndash;5pm during term time.

<!--The venue for this week’s seminar is **Room 739 at the <a href="https://www.openstreetmap.org/way/51517608" target=_blank>Institute of Education</a>**, 20 Bedford Way (note the change in venue from last term).<!--at <a href="https://www.openstreetmap.org/way/40205767" target=_blank>25, Gordon Street</a>.-->-->

To subscribe to the mailing list, please email Luke Collins on _luke [dot] collins [dot] 22 [at] ucl [dot] ac [dot] uk_.

---

# Next Speaker
<br>
<ul class="post-list">
{% capture currentDate %}
  {{ 'now' | date: '%s'}}
  {% endcapture %}
  {% for post in site.posts reversed %}
  {% capture postDate %}
  {{ post.date | date: '%s'}}
  {% endcapture %}
    {% if currentDate < postDate %}
    <!-- Don't show drafts -->
    <li>
      <h2>{{ post.title }} - <a href="{{ post.speaker-url }}">{{ post.speaker }}</a> ({{ post.speaker-uni }})</h2>
      <h2>{{ post.subtitle }}</h2>
      <br>
      <p>{{ post.excerpt }}</p>
      <br><br>
    </li>
    {%break%}
    {% else %}
    {% endif %}
  {% endfor %}
</ul>
