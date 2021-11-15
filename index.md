---
title: UCL Combinatorics seminar
---

The University College London (UCL) Combinatorics Seminar takes place weekly on Mondays, from 4pm to 5pm, at 25 Gordon Street (UCLU Building) Room 706. It is organised by [Shoham Letzter](http://www.homepages.ucl.ac.uk/~ucahsle/)  and [Alexey Pokrovskiy](https://alexeypokrovskiy.com). 

To subscribe to the mailing list, please email Shoham Letzter at s [dot] letzter [at] ucl [dot] ac [dot] uk.

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