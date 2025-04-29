---
layout: page
permalink: /program/
title: Program
description: (Tentative)
nav: true
nav_order: 6
---

<hr>
<!-- <h3>Workshop program</h3>
<ul> 
    <li>Introduction of the drafted journal structure that will serve as pivotal discussion guideline during the workshop</li>
    <li>Invited speakers' presentations followed by interactive activities to engage the audience and collect different perspectives on the topics</li>
    <li>Breakout sessions to discuss the topics in smaller groups</li>
    <li>Plenary session to present the results of the breakout sessions</li>
    <li>Panel session</li>
    <li>Closing remarks and definition of plan of action for the scientific contribution</li>
</ul> -->

<div class="card my-5" style="min-height: inherit; max-width: 50%; margin-left: auto !important; margin-right: auto !important;">
    <img src="/assets/img/program.png" class="mx-auto d-block" alt='program'>
</div>
The panel sessions are organized as <b>Oxford style</b> debates and panellists are invited to argue <b>FOR</b> or <b>AGAINST</b> the session topic. 
<br>
Stances are highlighted in each panellist card.
<hr>
<div style="text-align: center;">
      <p><a href="https://uni-augsburg.zoom-x.de/j/65783520158?pwd=bCC4HMEp86nk6Y9UbuXla31RIAugVB.1" class="btn main-button" target="_blank">Zoom Link</a></p>
    <p>Meeting ID: 657 8352 0158</p>
    <p>Passcode: sAS9=. </p>
</div>
<hr>
<h3>Panel session #1 - Personalization relinquishes user autonomy</h3>
<p><i>The design of personalised social robots must find a delicate balance between empowering the user and preserving their autonomy to avoid fostering overdependence and diminishing self-sufficiency.</i></p>
  <div id="myCarouselSpeakers" class="carousel container card-deck mt-3 mb-5">
    <div class="carousel-inner w-100 d-flex">  
        {% assign speakers_against = site.data.speakers.speakers | where: "session", "Session1" | where: "stance", "AGAINST" %}
        {% assign speakers_for = site.data.speakers.speakers | where: "session", "Session1" | where: "stance", "FOR" %}
        {% assign all_speakers = speakers_for | concat: speakers_against %}

        {% for speaker in all_speakers %}
            <div class="carousel-item {% if forloop.first %}active{% endif %}">
                <div class="col-md-3 my-1 pr-0 pl-0 h-100">
                    <div class="card p-1">
                        <a href="{{ speaker.website }}" target="_blank">
                            <img src="{{ speaker.image }}" class="card-img-top speaker-img" alt="{{ speaker.name }}">
                        </a>
                        <div class="card-body p-2">
                            <h5 class="card-title">{{ speaker.name }}</h5>
                            <p class="card-text">{{ speaker.title }}</p>
                            <p class="card-text">{{ speaker.affiliation }}</p>
                        </div>
                        <div class="card-footer text-muted small p-2">
                            {{ speaker.attendance }}
                        </div>
                        <div class="card-footer text-muted small p-2">Stance: {{ speaker.stance }}</div>
                    </div>
                </div>
            </div>
        {% endfor %}
    </div>

</div>

<hr>
<h3>Paper session (Accepted papers): </h3>
<i>5 min presentation + 2 min Q&amp;A</i>
<i>Schedule might be updated</i>
<ul>
    <li>"Exploring how users across cultures design and perceive multimodal robot emotion" - <i>Mathieu DePaul, Dagoberto Cruz-Sandoval and Alyssa Kubota</i></li>
    <li>"Personalising Explanations and Explaining Personalisation" - <i>Tamlin Love, Antonio Andriella and Guillem Alenyà</i></li>
    <li>"Learning Human-Robot Handshaking Preferences for Quadruped Robots" - <i>Alessandra Chappuis, Guillaume Bellegarda and Auke Ijspeert</i></li>
    <li>"Robots as Mediators to Resolve Multi-User Preference Conflicts" - <i>Aniol Civit, Rebecca Stower, Iolanda Leite, Antonio Andriella and Guillem Alenyà</i></li>
    <li>"EVOLVE: Emotion and Visual Output Learning via LLM Evaluation" - <i>Jordan Sinclair and Christopher Reardon</i></li>
    <li>"Detection of EEG ErrPs with no a priori knowledge of the occurrence time of stimuli" - <i>Alessandra Fava, Valeria Villani and Lorenzo Sabattini</i></li>
</ul>
<hr>
<h3>Coffee Break</h3>
<hr>

<h3>The Keynote Speaker: </h3>
<div class="row" style="display: flex; justify-content: center;">
  <div class="col-md-3 pr-0 pl-0 m-1" style = "min-height: 400px; max-width: 255px;">
      <div class="card p-1" style="min-height: inherit;">
        <a href="https://laurelriek.org/" target="_blank">
            <img src="/assets/img/lr.jpg" class="card-img-top speaker-img" alt="Lauriel Riek">
        </a>
        <div class="card-body p-2">
            <h5 class="card-title">Lauriel Riek</h5>
            <p class="card-text">Professor of Computer Science and Engineering</p>
            <p class="card-text">UC San Diego</p>
        </div>
        <div class="card-footer text-muted small p-2">
            In person <i class='fa-solid fa-user'></i>
        </div>
      </div>
  </div>
  <div class="col-md-6 m-1 pr-0 pl-0 d-inline">
      <div class="card p-1" style="min-height: inherit;">
      <div class="card-header"><h5>"Tempted by the promise of a different life": Technocratic Persuasion to Accept the Status Quo and Adopt Robots</h5></div>
      <div class="card-body"> <i>Abstract</i>: For a long time in robotics, we've perpetuated a techno-utopian future where robots seamlessly integrate into our lives, doing our chores, making our meals, taking on repetitive work - with the goal of freeing us up to do something better. We've worked tirelessly to convey this message, including trying to solve the “problem” of robot adoption via increasingly adaptive, interactive, and personalized robots. However, what happens if/when we get good at this? Despite our best intentions, we run the risk of our robots being used to reinforce the status quo, thus widening economic and health disparities for billions of people. This talk will explore key constructs from other disciplines to help frame these challenges, and discuss ways we roboticsts can pivot to better contextualize our work to help prevent dystopian narratives from coming to fruition.</div>
      </div>
  </div>
</div>

<hr>
<h3>Panel session #2 - Personalization reinforces social stereotypes and biases</h3>
<p><i>Personalised robots help adapt to user preferences and habits but at the same time they risk narrowing users' world-views and hinder opportunities for growth by overly customising experiences.</i></p>
<div id="myCarouselSpeakers" class="carousel container card-deck mt-3 mb-5">
    <div class="carousel-inner w-100 d-flex">  
        {% assign speakers_against = site.data.speakers.speakers | where: "session", "Session2" | where: "stance", "AGAINST" %}
        {% assign speakers_for = site.data.speakers.speakers | where: "session", "Session2" | where: "stance", "FOR" %}
        {% assign all_speakers = speakers_for | concat: speakers_against %}
        {% for speaker in all_speakers %}
            <div class="carousel-item {% if forloop.first %}active{% endif %}">
                <div class="col-md-3 my-1 pr-0 pl-0 h-100">
                    <div class="card p-1">
                        <a href="{{ speaker.website }}" target="_blank">
                            <img src="{{ speaker.image }}" class="card-img-top speaker-img" alt="{{ speaker.name }}">
                        </a>
                        <div class="card-body p-2">
                            <h5 class="card-title">{{ speaker.name }}</h5>
                            <p class="card-text">{{ speaker.title }}</p>
                            <p class="card-text">{{ speaker.affiliation }}</p>
                        </div>
                        <div class="card-footer text-muted small p-2">
                            {{ speaker.attendance }}
                        </div>
                        <div class="card-footer text-muted small p-2">Stance: {{ speaker.stance }}</div>
                    </div>
                </div>
            </div>
        {% endfor %}
    </div>
  </div>
<hr>
