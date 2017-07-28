---
layout: default
title: Past Speakers & Fellows
nav_title: Past Speakers & Fellows
mobile_nav_title: Alumni
permalink: /past-speakers-and-fellows/
order: 1
---

# Past Speakers
<div class="card-container">
{% for speaker in site.data.speakers %}
  {% if speaker.display == 'true' %}
    <div class="person-card">
      <div class="person-card-image-container">
        <img src="{{ site.baseurl }}/images/{{ speaker.image }}" />
      </div>
      <div class="person-card-text-container">
        <h3>{{ speaker.name }}</h3>
        <p>{{ speaker.bio }}</p>
      </div>
    </div>
  {% endif %}
{% endfor %}
</div>

# Cohort Leaders
<div class="card-container">
{% for leader in site.data.leaders %}
  <div class="person-card">
    <div class="person-card-image-container">
      <img src="{{ site.baseurl }}/images/{{ leader.image }}" />
    </div>
    <div class="person-card-text-container">
      <h3>{{ leader.name }}</h3>
      <p>{{ leader.cohorts }}</p>
    </div>
  </div>
{% endfor %}
</div>

# Fellows
<div class="card-container">
{% for fellow in site.data.fellows %}
  <div class="person-card">
    <div class="person-card-text-container no-image">
      <h3>{{ fellow.name }}</h3>
      <p>{{ fellow.cohort }}</p>
    </div>
  </div>
{% endfor %}
</div>

{% include cta.html %}
