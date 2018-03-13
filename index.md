---
layout: homepage
title: ""
description: "A team of F# experts that can offer you a complete range of services 
  including F# training, consulting, and functional-first development."
nav: "Home"
---

<div class="row" markdown="1">
<div class="col-md-4" markdown="1">
# Our services

We offer a complete range of services including training, F# consulting, and full project development.

We believe strongly in the benefits of using F#, but we also understand the challenges
around adding F# into your software development process.  Thats's why we offer training, support and other
services to make your use of F# as painless as possible.

[Read more about our workshops...](workshops.html)

</div>
<div class="col-md-4"  markdown="1">
# Our team

The **fsharpWorks** team has many years of experience solving real-world problems with F# in a wide range of areas
including finance, business application development, machine learning and other.

We are experts in integrating F#
into your software development mix, having written many of the definitive libraries, books, and blogs on these topics!

[Read more about the team...](team.html)

</div>
<div class="col-md-4"  markdown="1">
# Our technology

We think that F# is the best technology for you because it offers a unique combination of
correctness, time to market, efficiency and an ability to handle complex problems.

![F# Software Foundation](https://fsharpworks.com/images/fsharp_logo.png){:style="width:110px;float:right;margin:0px 0px 0px 15px"}
We are active members of the F# open-source community and we
are proud to support the F# Software Foundation as silver sponsors.

[Read testimonials from our customers...](testimonials.html)

</div>
</div>


<div class="row fw-events">
<div class="col-sm-7 fw-future">

  <h1 id="events">Upcoming events</h1>

  {% assign now = site.time | date: "%s" %}
  {% assign events = site.data.events | sort: "date" %}  
  {% for event in events %}  
    {% assign ed = event.date | date: "%s" %}
    {% if ed >= now %}
      <h3>{{ event.event }},
      {% if event.until <> nil %}
        {% assign m1 = event.date | date: "%b" %}
        {% assign m2 = event.until | date: "%b" %}
        {% if m1 == m2 %}{{ event.date | date: "%-d"}}-{{ event.until | date: "%-d"}} {{ event.date | date: "%b %Y"}}{% 
           else %}{{ event.date | date: "%-d %b"}} - {{ event.until | date: "%-d %b %Y"}}{% endif %}{% 
        else 
      %}{{ event.date | date: "%-d %b %Y"}}{% endif %}, {{ event.city }}</h3>
      <div class="row">
      <div class="col-sm-10">
        <p>{{ event.invite }}</p>
      </div>
      <div class="col-sm-2">
        <a href="{{ event.url }}" class="btn btn-primary" role="button">Register</a>
      </div>
      </div>
      <script type="application/ld+json">
      { 
        "@context": "http://schema.org",
        "@type": "EducationEvent",
        "location": { "@type": "Place", "name": "{{ event.city }}, {{ event.country }}", "address": "{{ event.city }}, {{ event.country }}" },
        "description": "{{ event.invite }}",
        "name": "{{ event.event }}",
        "startDate": "{{ event.date | date: "%F" }}",
        "endDate": "{% if event.until <> nil %}{{ event.until | date: "%F" }}{% else %}{{ event.date | date: "%F" }}{% endif %}",
        "url": "{{ event.url }}",
        "image": "https://fsharpworks.com/images/hp/1.jpg",
        "eventStatus": "http://schema.org/EventScheduled"
      }
      </script>      
    {% endif %}
  {% endfor %}

  <h3>F# in Finance - Online</h3>
  <div class="row">
  <div class="col-sm-10">
    <p>Join our 6-lecture online <a href="/workshops/finance.html">F# in Finance</a>
    any time and follow at your own pace, or contact us to arrange a private training.
    The workshop teaches practical functional concepts, data analysis with F# and more!</p>
  </div>
  <div class="col-sm-2">
    <a href="http://quantshub.com/content/self-paced-f-and-functional-programming-finance-tomas-petricek" class="btn btn-success" role="button">Join</a>
  </div>
  </div>

  <h3>Accessing Data with Type Providers - Online</h3>
  <div class="row">
  <div class="col-sm-10">
    <p>In this Pluralsight course by Tomas, you will learn how to easily
    call JSON-based REST services using type providers, package your F# code into a
    reusable .NET library, and integrate it into a C# ASP.NET application.</p>
  </div>
  <div class="col-sm-2">
    <a href="https://www.pluralsight.com/courses/accessing-data-fsharp-type-providers" class="btn btn-success" role="button">Join</a>
  </div>
  </div>

  <h3>On-site Private Training</h3>
  <div class="row">
  <div class="col-sm-10">
    <p>Do you want to gain practical hands-on F# skills? We offer private on-site trainings
    and consulting to fit your needs.</p>
  </div>
  <div class="col-sm-2">
    <a href="mailto:info@fsharpworks.com" class="btn btn-success" role="button">Contact us!</a>
  </div>
  </div>

<div class="fw-testimonials">
  <h1>Training testimonials</h1>
  <p>The fsharpWorks team has been providing F# trainings since 2011 and our attendees
  include many F# community leaders. <a href="testimonials.html">Learn more on our testimonials page!</a></p>

  <p class="fw-quote">
    "I attended a fsharpWorks 2-day F# course run by Phil and Tomas. (...) I would highly
    recommend this course for software developers that want to learn how to solve problems
    using functional programming techniques and quickly get up to speed with F#."
  </p>

  <p class="fw-quote-author">
    <a href="https://twitter.com/isaac_abraham/">Isaac Abraham</a>, F# MVP<br />
    Attended FastTrack to F# in 2012
  </p>
</div>

<h1>Our customers and partners</h1>

<p>Our customers include both large and small companies working in a wide range of areas
including finance and data analytics, security, enterprise software development,
research and many others.</p>

<div class="fw-logos fw-logos-hp">
  <a href="https://www.bluemountaincapital.com/"><img src="https://fsharpworks.com/images/partners/bmc.png" alt="BlueMountain Capital logo" /></a>
  <a href="http://www.danskebank.dk/"><img src="https://fsharpworks.com/images/partners/db.png" alt="Danske Bank logo" /></a>
  <a href="http://www.genetec.com/"><img src="https://fsharpworks.com/images/partners/genetec.png" alt="Genetec logo" /></a>
  <a href="http://www.microsoft.com/"><img src="https://fsharpworks.com/images/partners/msft.png" alt="Microsoft logo" /></a>
  <a href="http://research.microsoft.com/"><img src="https://fsharpworks.com/images/partners/msr.png" alt="Microsoft Research logo" /></a>
  <a href="http://www.skillsmatter.com/"><img src="https://fsharpworks.com/images/partners/skillsmatter.png" alt="Skills Matter logo" /></a>
  <a href="http://www.webstep.no/"><img src="https://fsharpworks.com/images/partners/webstep.png" alt="Webstep logo"/></a>
  <a href="http://broadrivercap.com/"><img src="https://fsharpworks.com/images/partners/broadriver.png" alt="BroadRiver logo"/></a>
</div>

</div> <!-- END # Col -->
<div class="col-sm-1"></div>
<div class="col-sm-4 fw-past">

<h1>News and updates</h1>
{% for item in site.data.news limit: 9 %}  
  <h3><a href="{{ item.url }}">{{ item.title }}</a></h3>
  {{ item.details | markdownify }}
{% endfor %}


</div> <!-- END # Col -->
</div> <!-- END # Row -->

<div class="row fw-events">
  <h1 style="margin:20px 0px 0px 15px">Past events</h1>  
  
  {% assign events = site.data.events | sort: "date" | reverse %}  
  {% assign now = site.time | date: "%s" %}
  {% assign futurecount = 0 %}
  
  {% for event in events %}
    {% assign ed = event.date | date: "%s" %}
    {% if ed >= now %}{% assign futurecount = futurecount | plus: 1 %}{% endif %}
  {% endfor %}
  
  {% for col in (1..3) %}
    <div class="col-sm-4">
    {% assign items = 10 %}
    {% assign offs = col | minus: 1 | times: items | plus: futurecount %}
    {% for event in events limit: items offset: offs %}  
      <h3>
      {% if event.until <> nil %}
        {% assign m1 = event.date | date: "%b" %}
        {% assign m2 = event.until | date: "%b" %}
        {% if m1 == m2 %}{{ event.date | date: "%-d"}}-{{ event.until | date: "%-d"}} {{ event.date | date: "%b %Y"}}{% 
           else %}{{ event.date | date: "%-d %b"}} - {{ event.until | date: "%-d %b %Y"}}{% endif %}{% 
        else 
      %}{{ event.date | date: "%-d %b %Y"}}{% endif %}, {{ event.city }}
      </h3>
      <p>
        {{ event.summary }}
      </p>
    {% endfor %}
    </div>
  {% endfor %}
</div>
