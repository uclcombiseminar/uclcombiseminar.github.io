---
title: UCL Combinatorics seminar
---

The University College London (UCL) Combinatorics Seminar is held every Monday at 4&ndash;5pm during term time.

The venue for this week’s seminar is Room LG16 at <a href="http://www.ucl.ac.uk/maps/ioe" target=_blank>20, Bedford Way</a>.

To subscribe to the mailing list, please email Luke Collins at luke [dot] collins [dot] 22 [at] ucl [dot] ac [dot] uk.

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
