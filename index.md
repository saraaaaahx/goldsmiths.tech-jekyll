---
title: Home
projectname: home
layout: default
og: og.png
one_line: Hacksmiths is the award-winning student-run tech society at Goldsmiths, University of London.
---

<section class="switchable feature-large bg--secondary hero">
    <div class="container">
        <div class="row">
            <div class="col-sm-6 col-md-5">
                <div class="switchable__text">
                    <img src="/assets/img/logo-hacksmiths.svg" alt="Hacksmiths Logo">
                    <p class="lead"> Hacksmiths is the student-run tech society at Goldsmiths. Our mission is to provide an opportunity for people in all departments and from all backgrounds the chance to learn about, and play with, technology. </p>
                    <a class="btn btn--sm btn--primary type--uppercase" href="/join"> <span class="btn__text">Become a member - join for free</span> </a>
                    <br>
                    <a href="//www.youtube.com/watch?v=pkHNc2wiNxI" class="btn btn--sm type--uppercase" data-lity>
                        <i class="socicon icon socicon-youtube"></i>
                        <span>What we do</span>
                    </a>
                    <a href="https://m.me/smithsbot" class="btn btn--sm type--uppercase" target="_blank">
                        <i class="socicon icon socicon-messenger"></i>
                        <span>Get updates</span>
                    </a>
                </div>
            </div>
            <div class="col-sm-6">
                <div class="boxed boxed--lg boxed--border">
                    <div class="feature feature-2">
                        <div class="feature__body">
                            <h5>Weekly Code &amp; Craft</h5>
                            <p>A friendly and supportive environment to play around with new ideas and get support. Suitable for all skill levels.<br></p>
                        </div>
                    </div>
                    <div class="feature feature-2">
                        <div class="feature__body">
                            <h5>Monthly talks &amp; workshops</h5>
                            <p> A range of interesting content from students, staff and industry professionals. Suitable for complete beginners.</p>
                        </div>
                    </div>
                    <div class="feature feature-2">
                        <div class="feature__body">
                            <h5>Hackathons &amp; jams</h5>
                            <p>Invention marathons which bring together people with varying skills to build awesome projects. Suitable for all skill levels.</p>
                        </div>
                    </div>
                    <div class="feature feature-2">
                        <div class="feature__body">
                            <h5>Lovelace</h5>
                            <p>A social event series for women and non binary people interested in technology at goldsmiths. Suitable for all skill levels.</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</section>

<section class="events">
    <div class="container">
        <div class="row">
            <h2>Our events</h2>
            {% for event in site.data.events %}
                <div class="col-sm-4 event-single">
                    <a {% unless event.url == "undefined" %} href="{{event.url}}" {% endunless %}>
                        <div class="feature feature-1">
                            <div class="feature__body boxed boxed--border">
                                {% if event.past %}<span>Past</span>{% endif %}
                                <h5>{{event.name}}</h5>
                                <p>{{event.line}}</p>
                                <small>{{event.date}}</small>
                            </div>
                        </div>
                    </a>
                </div>
            {% endfor %}
        </div>
        <h3><a href="https://calendar.google.com/calendar/embed?src=jellybabi.es_l70qvq3qcvbe4sci1pskevfu4c%40group.calendar.google.com&ctz=Europe/London">Click here for a full calendar which you can import to your own apps.</a></h3>
    </div>
</section>

{% include valuable-skills.html %}
