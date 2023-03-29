---
layout: default
meta-description: "LoG$^\text{2}$: Learning on Graphs and Geometry @ Oxford"
---

# LoG$^\textbf{2}$ @ Oxford
The **Learning on Graphs and Geometry** seminar series at the University of Oxford is a forum for discussing recent advances in the field of geometric deep learning, which lies at the intersection of machine learning and geometry. The group focuses on exploring the theoretical foundations and practical applications of graph neural networks, manifold learning, and other techniques for processing and analyzing data with a non-Euclidean structure. Members of the group include researchers and graduate students from various departments, including Computer Science, Engineering, Mathematics, and Statistics, who share an interest in developing novel machine learning methods for understanding complex data sets with graph or geometric structure .

The seminar series takes place biweekly on Thursday 14:00-15:00 in Room C5 at the Mathematical Institute (Andrew Wiles building). To join online, please use the Zoom link <a href="https://us06web.zoom.us/j/86881074813?pwd=UEpYU1UyTTF3a3kwL3F5VkFjdkZ6QT09">here</a>.

To subscribe to our mailing list, you can send an email <a href="mailto: log2-subscribe@maillist.ox.ac.uk">here</a>. 



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
