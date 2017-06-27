---
layout: page
title: "Books and talks"
description: "F# books written by our team and recordings of our conference talks."
nav: "Materials"
banner1: "Did some topic catch your interest and you want to learn more? Many our talks are based on the content that we cover in our <a href='workshops.html'>practical hands-on workshops</a>!"
bannerImage: img5
---

<div class="row fw-statement" markdown="1">

Are you just getting started with functional programming? Or are you interested in using it in practice
for web, development, enterprise applications, finance or data science? Here, you'll find our books and
high-quality recordings of our talks.

* [Getting started with F# in practice](#getting-started)
* [Machine learning and data science](#mlds)
* [Web development and cloud services](#web)
* [Using F# in the enterprise & architecture](#enterprise)
* [Functional, compilers, performance & fun!](#fun)

</div>

<div class="row" markdown="1">
  <div class="col-md-12" markdown="1" style="margin:0px 0px 0px 0px">
  <a name="getting-started">

### Getting started with F# in practice
            
Functional programming languages are good at expressing complex ideas in a succinct,
declarative way. Functional concepts such as "immutability" and "function values" make
it easier to reason about code - as well as helping with concurrency. F#, LINQ, and
numerous .NET libraries now bring the power of functional programming to .NET coders.

Materials in this section teach the ideas and techniques of functional programming applied
to real-world problems. You'll see how the functional way of thinking changes the game
for .NET developers. 

  </div>
</div>

<div class="row fw-materials" markdown="1">
  <div class="col-sm-2 book-image hidden-xs">
    <a href="http://functional-programming.net/rwfp/"><img src="images/books/rwfp.png" class="img-responsive" /></a>
  </div>
  <div class="col-sm-10" markdown="1">

### [Real-World Functional Programming](http://functional-programming.net/rwfp/)

<p class="book-author">Tomas Petricek with Jon Skeet, Manning, 2012</p>

Written by Tomas Petricek with Jon Skeet, this best-selling tutorial teaches the ideas and
techniques of functional programming applied to real-world problems. You'll see how the
functional way of thinking changes the game for .NET developers. Then, you'll tackle common
issues using a functional approach. The book will also teach you the basics of the F#
language and extend your C# skills into the functional domain.


> *"You will never look at your code in the same way again."* <br /> 
> from the foreword by Mads Torgersen, C# PM, Microsoft

  </div>
</div>  

<div class="row fw-materials">
  <div class="col-sm-2 book-image hidden-xs">
    <a href="http://www.gitbook.com/book/swlaschin/fsharpforfunandprofit/"><img src="images/books/funprof.png" class="img-responsive" /></a>
  </div>
  <div class="col-sm-10" markdown="1">

### [F# for Fun and Profit (e-book)](http://www.gitbook.com/book/swlaschin/fsharpforfunandprofit/)

<p class="book-author">Scott Wlaschin</p>

The e-book version of Scott's <a href="http://fsharpforfunandprofit.com">fsharpforfunandprofit.com</a> web site.
Perfect if you want to browse the site offline while commuting or on a flight.
The site (and this book) aims to introduce you to F# and show you ways that F# can help in day-to-day development of mainstream commercial business software. On the way, I hope to open your mind to the joys of functional programming - it really is fun!                              

> *"The best teacher there is of functional programming concepts"*<br />
> Larry O'Brien, founding editor of Software Development magazine

  </div>
</div>  

<div class="row fw-materials">
  {% assign talks = site.data.talks | sort: "year" | reverse %}  
  {% for item in talks %}  
    {% if item.category == 'intro' %}
    <div class="col-lg-2 col-md-2 col-sm-4 col-xs-3 fw-talk">
      <div class="img-wrapper"><a href="{{ item.link }}"><img src="images/talks/{{ item.image }}" class="img-responsive" /></a>
    </div></div>
    <div class="col-lg-4 col-md-4 col-sm-8 col-xs-9 fw-talk">
      <h4><a href="{{ item.link }}">{{ item.title }}</a></h4>
      <p class="author">{{ item.author }}, {{ item.event }} {{ item.year }}</p>
      <p class="about">{{ item.about }}</p>
    </div>
    {% endif %}
  {% endfor %}
</div>


<div class="row fw-materials" markdown="1">
<div class="col-md-12" style="margin:0px 0px 0px 0px" markdown="1">
<a name="mlds">

## Machine learning and data science

Machine learning (ML) is becoming an extremely important topic and F# is the perfect
tool for doing ML (not just) on the .NET platform. Books and talks in
this category give you all the information you need to get started with using F# for
data science and machine learning.

F# is a great fit for implementing your efficient own algorithms, but it can also access
a wide range of powerful libraries including <a href="http://www.fslab.org">FsLab</a>
for data science, <a href="http://www.mbrace.io">MBrace</a> for extreme scalability
and <a href="http://bluemountaincapital.github.io/FSharpRProvider/">R through the R type provider</a>.

</div>
<div class="row fw-materials" markdown="1"> 
<div class="col-sm-2 book-image hidden-xs">
  <a href="http://www.amazon.com/dp/1430267674/"><img src="images/books/mlproj.jpg" class="img-responsive" /></a>
</div>
<div class="col-sm-10" markdown="1">

### [Machine Learning Projects for .NET Developers](http://www.amazon.com/dp/1430267674/)

<p class="book-author">Mathias Brandewinder, Apress, 2015</p>

The book shows you how to build smarter .NET applications that learn from data, using simple
algorithms and techniques that can be applied to a wide range of real-world problems. You'll
code each project in the familiar setting of Visual Studio, while the machine learning logic
uses F#, a language ideally suited to machine learning applications in .NET. If you're new to
F#, this book will give you everything you need to get started. If you're already familiar
with F#, this is your chance to put the language into action in an exciting new context.

> *"Awesome read! The book explains ML concepts in a very easy and compelling
  manner, with great and well explained codes samples."* Amazon review by
  [Terrell Bryonyq](http://www.amazon.com/gp/customer-reviews/R5N3XU9GE3SCQ/ref=cm_cr_arp_d_rvw_ttl?ie=UTF8&ASIN=1430267674)
  
  </div>
</div>

<div class="row fw-materials"> 
  <div class="col-sm-2 book-image hidden-xs">
    <a href="http://fslab.org/report/"><img src="images/books/fslab.png" class="img-responsive" /></a>
  </div>
  <div class="col-sm-10" markdown="1">

### [Analyzing and Visualizing Data with F#](http://fslab.org/report/)

<p class="book-author">Tomas Petricek, O'Reilly, 2015 (free report)</p>

In this report, F# contributor Tomas Petricek explains many of the key features of the F#
language that make it a great tool for data science and machine learning. Real world examples
take you through the entire data science workflow with F#, from data access and analysis to presenting the results. 

You'll learn about how F# and its unique features ease the chore of data access,
the process of data analysis and visualization, using Deedle, R type provider and XPlot and
finally, implementations for a clustering algorithm using the standard F# library and how the F# type inference helps you understand your code.

  </div>
</div>
<div class="row fw-materials">
  {% assign talks = site.data.talks | sort: "year" | reverse %}  
  {% for item in talks %}  
    {% if item.category == 'ml' %}
    <div class="col-lg-2 col-md-2 col-sm-4 col-xs-3 fw-talk">
      <div class="img-wrapper"><a href="{{ item.link }}"><img src="images/talks/{{ item.image }}" class="img-responsive" /></a>
    </div></div>
    <div class="col-lg-4 col-md-4 col-sm-8 col-xs-9 fw-talk">
      <h4><a href="{{ item.link }}">{{ item.title }}</a></h4>
      <p class="author">{{ item.author }}, {{ item.event }} {{ item.year }}</p>
      <p class="about">{{ item.about }}</p>
    </div>
    {% endif %}
  {% endfor %}
</div>
<div class="row fw-materials">
  <div class="col-md-12" style="margin:0px 0px 0px 0px" markdown="1">
  <a name="web">

## Web development and cloud services

One of the myths about F# is that it is only good for complex mathematics. This could
not be further from truth. A web server is essentially a function from a request to a
response and so functional programming is a perfect fit for it.

Talks in this category cover some of the most popular F# tools for doing web development
including the functional cross-platform web server <a href="http://www.suave.io">Suave</a>,
but you can also learn about building and hosting cloud-based services on Azure.

  </div>
</div>
<div class="row fw-materials">
  {% assign talks = site.data.talks | sort: "year" | reverse %}  
  {% for item in talks %}  
    {% if item.category == 'web' %}
    <div class="col-lg-2 col-md-2 col-sm-4 col-xs-3 fw-talk">
      <div class="img-wrapper"><a href="{{ item.link }}"><img src="images/talks/{{ item.image }}" class="img-responsive" /></a>
    </div></div>
    <div class="col-lg-4 col-md-4 col-sm-8 col-xs-9 fw-talk">
      <h4><a href="{{ item.link }}">{{ item.title }}</a></h4>
      <p class="author">{{ item.author }}, {{ item.event }} {{ item.year }}</p>
      <p class="about">{{ item.about }}</p>
    </div>
    {% endif %}
  {% endfor %}
</div>

<div class="row fw-materials">
  <div class="col-md-12" style="margin:0px 0px 0px 0px" markdown="1">
  <a name="enterprise">

## Using F# in the enterprise & architecture

F# is a great language for developing enterprise applications in various domains including
retail, advertising, finance and many more. The functional-first nature of the F# language leads you towards the "happy path" of
correctness and extensibility.

The materials in this section provide all you need to build the right functional architecture. You can watch
Scott Wlaschin's amazing series of talks on functional patterns or explore a number of case studies
of using F# in the industry.

  </div>
</div>

<div class="row fw-materials">
  <div class="col-sm-2 book-image hidden-xs">
    <a href="http://functional-programming.net/deepdives/"><img src="images/books/deep.png" class="img-responsive" /></a>
  </div>
  <div class="col-sm-10">
    <h3><a href="http://functional-programming.net/deepdives/">F# Deep Dives</a></h3>
    <p class="book-author">Edited by Tomas Petricek and Phil Trelford, Manning, 2014</p>

    <p>F# Deep Dives presents a collection of real-world F# techniques, each written by
      expert practitioners. Each chapter presents a new use case where you'll read how the author
      used F# to solve a complex problem more effectively than would have been possible using
      a traditional approach. You'll not only see how a specific solution works in a specific
      domain, you'll also learn how F# developers approach problems, what concepts they use to
      solve them, and how they integrate F# into existing systems and environments.</p>

    <p class="quote"><em>"Outstanding real-world examples that are sure to appeal to both the novice and expert."</em><br />
      Jeff Smith ITT Education Services</p>
  </div>
</div>

<div class="row fw-materials">
  {% assign talks = site.data.talks | sort: "year" | reverse %}  
  {% for item in talks %}  
    {% if item.category == 'enterprise' %}
    <div class="col-lg-2 col-md-2 col-sm-4 col-xs-3 fw-talk">
      <div class="img-wrapper"><a href="{{ item.link }}"><img src="images/talks/{{ item.image }}" class="img-responsive" /></a>
    </div></div>
    <div class="col-lg-4 col-md-4 col-sm-8 col-xs-9 fw-talk">
      <h4><a href="{{ item.link }}">{{ item.title }}</a></h4>
      <p class="author">{{ item.author }}, {{ item.event }} {{ item.year }}</p>
      <p class="about">{{ item.about }}</p>
    </div>
    {% endif %}
  {% endfor %}
</div>

<div class="row">
  <div class="col-md-12" style="margin:0px 0px 0px 0px">
    <a name="fun"></a><h2>Functional, compilers, performance &amp; fun!</h2>
    <p>Do you want to learn more about functional programming and F#? Then the talks in this section are the
      place to explore! Learn about more advanced functional programming concepts (did we say <em>monads</em>?),
      techniques for choosing the right data structure, compilers, but also some of the powerful F# libraries
      like <a href="http://tpetricek.github.io/FSharp.Formatting">F# Formatting</a> and the awesome tool for
      building presentations called <a href="http://fsprojects.github.io/FsReveal/">FsReveal</a>.
    </p>
  </div>
</div>
<div class="row fw-materials">
  {% for item in site.data.talks %}  
    {% if item.category == 'fun' %}
    <div class="col-lg-2 col-md-2 col-sm-4 col-xs-3 fw-talk">
      <div class="img-wrapper"><a href="{{ item.link }}"><img src="images/talks/{{ item.image }}" class="img-responsive" /></a>
    </div></div>
    <div class="col-lg-4 col-md-4 col-sm-8 col-xs-9 fw-talk">
      <h4><a href="{{ item.link }}">{{ item.title }}</a></h4>
      <p class="author">{{ item.author }}, {{ item.event }} {{ item.year }}</p>
      <p class="about">{{ item.about }}</p>
    </div>
    {% endif %}
  {% endfor %}
</div>

<div class="row">
  <div class="col-md-12">
    <h1>Conferences and publishers</h1>
    <p>
      Over the years, we had the pleasure of speaking at a number of conferences and working
      with several publishers. If you are interested in meeting in person, you'll often find
      us at events organized by our partners listed here. Are you interested in having
      fsharpWorks experts at your event?
      <a href="mailto:info@fsharpworks.com">Drop us an email to discuss what we can do for you!</a>
    </p>

    <div class="fw-logos fw-logos-detail">
      <a href="http://www.skilsmatter.com/"><img src="images/partners/skillsmatter.png" alt="Skills Matter"/></a>
      <a href="http://www.lambdadays.org/"><img src="images/partners/lambda.png" alt="Lambda Days"/></a>
      <a href="http://www.ndc-oslo.com/"><img src="images/partners/ndc.png" alt="NDC Oslo and London"/></a>
      <a href="http://channel9.msdn.com/"><img src="images/partners/ch9.png" alt="Channel 9"/></a>
      <a href="http://www.apress.com/"><img src="images/partners/apress.png" alt="Apress"/></a>
      <a href="http://www.codemesh.io/"><img src="images/partners/cm.png" alt="Code Mesh"/></a>
      <a href="http://www.manning.com/"><img src="images/partners/manning.png" alt="Manning"/></a>
    </div>
  </div>
</div>
