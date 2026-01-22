---
title: UCL Combinatorics Seminar
---

The University College London (UCL) Combinatorics Seminar is held every Monday at 4&ndash;5pm during term time.

The venue for seminars this term is **Room 346 at the <a href="https://www.openstreetmap.org/way/40253190" target=_blank>SSEES Bulding</a>**, 14–16 Taviton Street.<!--at <a href="https://www.openstreetmap.org/way/40205767" target=_blank>25, Gordon Street</a>.-->

To subscribe to the mailing list, please email Luke Collins on _luke [dot] collins [dot] 22 [at] ucl [dot] ac [dot] uk_.

---

# Next Speaker
<br>
<ul class="post-list">
  {% assign today_num = 'now' | date: '%Y%m%d' %}
  {% for post in site.posts reversed %}
    {% assign post_num = post.date | date: '%Y%m%d' %}
    {% if post_num >= today_num %}
      <li>
        <h2>{{ post.title }} - <a href="{{ post.speaker-url }}" target=_blank>{{ post.speaker }}</a> ({{ post.speaker-uni }})</h2>
        <h2>{{ post.subtitle }}</h2>
        <br>
        <p>{{ post.excerpt }}</p>
        <br><br>
      </li>
      {% break %}
    {% endif %}
  {% endfor %}
</ul>
