---
layout: default
meta-description: "LoG$^\text{2}$: Learning on Graphs and Geometry @ Oxford"
---

# LoG$^\textbf{2}$ @ Oxford
The **Learning on Graphs and Geometry** reading group at the University of Oxford is a forum for discussing recent advances in the field of geometric deep learning, which lies at the intersection of machine learning and geometry. The group focuses on exploring the theoretical foundations and practical applications of graph neural networks, manifold learning, and other techniques for processing and analyzing data with a non-Euclidean structure. Members of the group include researchers and graduate students from various departments, including computer science, mathematics, and engineering, who share an interest in developing novel machine learning methods for understanding complex data sets with graph or geometric structure.




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

**Organisers (Students):** Álvaro Arroyo, Shazia Babul, Federico Barbero, Ben Finkelshtein, Yixuan He, Emily Jin, Haitz Sáez de Ocáriz Borde
