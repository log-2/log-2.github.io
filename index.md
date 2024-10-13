---
layout: default
meta-description: "Oxford - Learning on Graphs and Geometry"
---

The **Learning on Graphs and Geometry** seminar series at the University of Oxford is a forum for discussing recent advances in the field of geometric deep learning, which lies at the intersection of machine learning and geometry. The group focuses on exploring the theoretical foundations and practical applications of graph neural networks, manifold learning, and other techniques for processing and analyzing data with a non-Euclidean structure. Members of the group include researchers and graduate students from various departments, including Computer Science, Engineering, Mathematics, and Statistics, who share an interest in developing novel machine learning methods for understanding complex data sets with graph or geometric structure.

The seminar series will normally take place biweekly during term time. Please look out for talk announcements for the exact time and location. To receive announcements, please subscribe to our mailing list by sending an email <a href="mailto: log2-subscribe@maillist.ox.ac.uk">here</a>. 



{% for category in site.data.talks %}
# {{ category.type }}
<div class="talk-list">
  {% for talk in category.members %}
  <div class="talk list-group-item">
  <div class="talk-date">{{ talk.date }}</div>
  <div class="talk-presenter">{{ talk.speaker }}</div>
  {% if talk.title %}
  <div>
    {% if talk.recording %}
      <span><a class="talk-title-link" href="{{ talk.recording }}">{{ talk.title }} <i class="bi bi-box-arrow-up-right"></i></a></span>
    {% elsif talk.livestream %}
      <span><a class="talk-title-link" href="{{ talk.livestream }}">{{ talk.title }} <i class="bi bi-box-arrow-up-right"></i></a></span>
    {% else %}
      <span>{{ talk.title }}</span>
    {% endif %}
  </div>
  {% endif %}
  {% if talk.abstract %}
    <details>
    <summary>Abstract</summary>
    {{ talk.abstract }}
    
    {% if talk.bio %}
    <br><br>
    <strong>Bio: </strong> {{ talk.bio }}
    {% endif %}

    {% if talk.recording %}
      <br><br>
      <strong><a href="{{ talk.recording }}">Video Link</a></strong>
    {% elsif talk.livestream %}
      <br><br>
      <strong><a href="{{ talk.livestream }}">Livestream Link</a></strong>
    {% endif %}
    </details>
  {% endif %}
  </div>
  {% endfor %}
</div>
{% endfor %}

# About 

**Organisers (Faculty):** <a href="https://www.cs.ox.ac.uk/people/michael.bronstein/">Michael Bronstein</a>, <a href="https://www.cs.ox.ac.uk/people/ismaililkan.ceylan/">Ismail Ilkan Ceylan</a>, <a href="https://www.stats.ox.ac.uk/~cucuring/">Mihai Cucuringu</a>, <a href="https://web.media.mit.edu/~xdong/">Xiaowen Dong</a>, <a href="https://www.cs.ox.ac.uk/people/ismaililkan.ceylan/"><a href="https://www.maths.ox.ac.uk/people/renaud.lambiotte">Renaud Lambiotte</a>

**Organisers (Students):** Álvaro Arroyo, Jacob Bamberger, Federico Barbero, Ben Finkelshtein,  Emily Jin
