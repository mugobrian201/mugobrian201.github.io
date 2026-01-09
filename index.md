---
layout: splash
permalink: /
header:
  overlay_color: "#5e616c"
  overlay_image: /assets/images/home-bg.jpg  # We'll add a subtle background later
  cta_label: "View My Projects"
  cta_url: /projects/
  caption: "Building predictive models that solve real-world problems in Africa and beyond"
excerpt: >
  <p style="font-size:1.2em">Actuarial Science graduate specializing in machine learning solutions for disaster response, urban planning, and environmental health. Currently expanding my skills through WorldQuant University's Applied Data Science Lab.</p>
feature_row:
  - image_path: /assets/images/mexico-project-thumb.jpg
    alt: "Mexico Real Estate Analysis"
    title: "Property Value Drivers"
    excerpt: "Identified key factors influencing Mexican real estate prices using spatial analysis"
    url: "/projects/#mexico-real-estate-analysis"
    btn_class: "btn--primary"
    btn_text: "Explore Project"
  - image_path: /assets/images/nepal-project-thumb.jpg
    alt: "Nepal Earthquake Prediction"
    title: "Disaster Response Modeling"
    excerpt: "Predicted building damage severity to optimize emergency resource allocation"
    url: "/projects/#nepal-earthquake-damage-prediction"
    btn_class: "btn--primary"
    btn_text: "Explore Project"
---

{% include feature_row id="intro" type="center" %}

<div class="feature__wrapper">
  <h2 class="archive__subtitle">Featured Technical Skills</h2>
  <div class="grid__wrapper">
    {% for skill in site.data.skills %}
    <div class="grid__item">
      <div class="card">
        <div class="card__image">
          <i class="fas fa-{{ skill.icon }} fa-3x"></i>
        </div>
        <div class="card__content">
          <h3 class="card__title">{{ skill.name }}</h3>
          <p class="card__text">{{ skill.description }}</p>
        </div>
      </div>
    </div>
    {% endfor %}
  </div>
</div>
