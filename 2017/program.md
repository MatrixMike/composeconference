---
layout: 2017/page
title: C◦mp◦se 2017 Program
permalink: /2017/program/
---

Register for C◦mp◦se :: Conference 2017 tickets at [composeconference.eventbrite.com](http://composeconference.eventbrite.com)

---

<!-- Thursday's schedule -->
## Thursday, May 18, 2017

<table class="table table-bordered" style="background: #fff">
    <tr class="active"><th width="200">Time</th><th>Talk</th></tr>
    <tr>
    <tr><td>8:30am - 9:00am</td><td>Registration</td></tr>
    <td>9:00am - 9:45am</td>
    <td>
        <p class="lead">
          <b>KEYNOTE: A categorical view of computational effects</b> <br/>
            <small>
             Dr. Emily Riehl
            </small>
        </p>
        <blockquote class="abstract">
Monads have famously been used to model computational effects, although, curiously, the computer science literature presents them in a form that is scarcely recognizable to a category theorist — I’d say instead that a monad is just a monoid in the category of endofunctors, what’s the problem? ;) To a categorical eye, computational effects are modeled using the Kleisli category of a monad, a perspective which suggests another categorical tool that might be used to reason about computation. The Kleisli category is closely related to another device for categorical universal algebra called a Lawvere theory, which may be a more natural framework to model computation (an idea suggested by Gibbons, Hinze, Hyland, Plotkin, Power and certainly others). This talk will survey monads, Lawvere theories, and the relationships between them and illustrate the advantages and disadvantages of each framework through a variety of examples: lists, exceptions, side effects, input-output, probabilistic non-determinism, and continuations.
</blockquote>
</td></tr>

{% assign sorted = (site.data.2017.speakers.speakers | sort: 'start_time') %}

{% for speaker in sorted %}
  {% if speaker.start_time <= '2017-05-18 18:00:00 -0500' %}
    <tr id="{{speaker.name}}">
      <td>{{ speaker.start_time | date: '%I:%M%P' }} - {{ speaker.end_time | date: '%I:%M%P' }}</td>
      <td>
        <p class="lead">
          <b>{{ speaker.title }}</b> <br/>
            <small>
                {{ speaker.name }}
            </small>
        </p>
        <blockquote class="abstract">
            {{ speaker.abstract | markdownify }}
        </blockquote>
      </td>
    </tr>
  {% endif %}
{% endfor %}
</table>


<!-- Friday's schedule -->
## Thursday, May 19, 2017

<table class="table table-bordered" style="background: #fff">
    <tr class="active"><th width="200">Time</th><th>Talk</th></tr>


{% for speaker in sorted %}
  {% if speaker.start_time >= '2017-05-18 18:00:00 -0500' %}
    <tr id="{{speaker.name}}">
      <td>{{ speaker.start_time | date: '%I:%M%P' }} - {{ speaker.end_time | date: '%I:%M%P' }}</td>
      <td>
        <p class="lead">
          <b>{{ speaker.title }}</b> <br/>
            <small>
                {{ speaker.name }}
            </small>
        </p>
        <blockquote class="abstract">
            {{ speaker.abstract | markdownify }}
        </blockquote>
      </td>
    </tr>
 {% endif %}
{% endfor %}
</table>



---

Register for C◦mp◦se :: Conference 2017 tickets at [composeconference.eventbrite.com](http://composeconference.eventbrite.com)
