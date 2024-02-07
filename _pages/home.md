---
layout: default
permalink: /
title: Home
nav: true
nav_order: 1
img: think.jpg
pagination:
  enabled: true
  collection: posts
  permalink: /page/:num/
  per_page: 5
  sort_field: date
  sort_reverse: true
  trail:
    before: 1 # The number of links before the current page
    after: 3 # The number of links after the current page
---
<link rel="stylesheet" href="{{ site.baseurl | prepend: site.url }}/custom.css">
<div class="post">

{% assign blog_name_size = site.blog_name | size %}
{% assign blog_description_size = site.blog_description | size %}

  <div class="header-bar">
    <h1>{{ site.blog_name }}</h1>
    <h2>{{ site.blog_description }}</h2>
  </div>

  <div class="tag-category-list">
    <ul class="p-0 m-0">      
        <li>
          <i class="fa-solid fa-hashtag fa-sm"></i> <a href="https://www.ro-man2024.org/" target=_blank>roman24</a>
        </li>
          <p>&bull;</p>
          <i class="fa-solid fa-pin fa-sm"></i> <p> 26th August 2024</p>
        <p>&bull;</p>
        <i class="fa fa-place" aria-hidden="true"></i> <p> Pasadena California, USA</p>
    </ul>
  </div>
  

<!-- <div style="text-align: center;"><p><h3>Personalisation in robotics is...</h3></p></div> -->
<!-- <div style="margin-top: -15px; text-align: center;"><p><h3><span id="typing-text"></span></h3></p></div> -->
</div>

<div class="row m-3">
<div class="col-sm-9">
<h3>Abstract</h3>
<p class="main-description">
The importance of personalisation in Human-Robot Interaction has already shown its advantages in multiple scenarios and will become a prevalent direction for the field.
Robots are required to adapt their behaviour in both short- and long-term interactions.
In the short term, as the interactions are very often limited in time, robots need to learn from scratch the user's preferences and adapt quickly to them. In the long term, users' needs may change and robots need to continuously adapt in a way that keeps them engaged and interested over time.
Personalisation can greatly improve short- and long-term interactions in various real-world scenarios by fostering trust and rapport, increasing adherence to the interaction, enhancing engagement through tailored content, and improving task performance. 
Nonetheless, it is essential to consider whether and to what extent personalisation can be beneficial for interactions and users. Robots developed as end-to-end systems for conducting social interactions can amplify cultural biases, gender and age stereotypes. Therefore, it is crucial to discuss when personalisation is desired or required, and when it should be avoided. 
In contexts such as healthcare and education, personalisation can lead to inadequate care or support and lower acceptance of the professionals who use the technology (teachers and healthcare professionals). Additionally, collecting personal data to provide tailored assistance can raise privacy concerns, as many machine learning algorithms are not transparent to users. Furthermore, deep learning algorithms may amplify existing biases, hindering the primary goal of making interactions more engaging and trustworthy.


The workshop focuses on the benefits and drawbacks of personalisation and behavioural adaptation in social HRI. In particular, this workshop aims at bringing together a multidisciplinary group of researchers from areas including, but not limited to, psychology, neuroscience, computer science, robotics, and sociology, to share and discuss current approaches for robots specifically designed for meeting the individual's unique needs via adaptive behaviours and learning capabilities.

</p>
</div>
<div class="col-sm-3">

{% if page.img %}
  <img class="caption__media" data-interchange="
  {% for img in page.img %}
    [{{site.baseurl}}/asset/img/{{img[1]}} ({{img[0]}})]
    {% unless forloop.last %}, {% endunless %}
  {% endfor %}
  ">
{% endif %}

<img class="card-img" src="{{ site.baseurl }}/assets/img/{{ page.img }}" alt="image">

</div>

</div>

<div class="tag-category-list">
    <ul class="p-0 m-0">
        <p>&bull;</p>
    </ul>
  </div>
  <hr>
</div>
