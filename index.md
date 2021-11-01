---
title: UCL Combinatorics seminar
---

The University College London (UCL) Combinatorics Seminar takes place weekly on Mondays, from 4pm to 5pm, at 25 Gordon Street (UCLU Building) Room 706. It is organised by [Shoham Letzter](http://www.homepages.ucl.ac.uk/~ucahsle/)  and [Alexey Pokrovskiy](https://alexeypokrovskiy.com). 

To subscribe to the mailing list, please email Shoham Letzter at s [dot] letzter [at] ucl [dot] ac [dot] uk.

---

# Next Speaker
<br>
<ul class="post-list">
  {% for post in site.posts reversed %}
    {% if post.title contains '8 November' %}
    <li>
      <h2>{{ post.title }} - <a href="{{ post.speaker-url }}">{{ post.speaker }}</a> ({{ post.speaker-uni }})</h2>
      <h2>{{ post.subtitle }}</h2>
      <br>
      <p>{{ post.excerpt }}</p>
    </li>
    <!-- Don't show other talks -->
    {% else %}
        {% endif %}
  {% endfor %}
</ul>
