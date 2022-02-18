---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home

---

<h2>A.M. 235452</h2>
<h2>Personal Information</h2>


<ul>
    <li><strong>Name:</strong> {{ site.data.personal.name }}</li>
    <li><strong>Email:</strong> {{  data.personal.email }}</li>
    <li><strong>Date of Birth:</strong> {{ site.data.personal.birthday }}</li>
    <li><strong>City:</strong> {{ site.data.personal.city }}</li>
    <li>
        <strong>LinkedIn link:</strong> 
        <a href="http://{{ site.data.personal.linkedin }}" target="_blank">{{site.data.personal.linkedin}}</a>
    </li>
    <li>
        <strong>GitHub link:</strong>
        <a href="http://{{ site.data.personal.github }}" target="_blank">{{site.data.personal.github}}</a>
    </li>
</ul>

_______________________


<h2>Education</h2>

<ul>
    {% for edu in site.data.education.education %}
        <li><strong>Period time:</strong> {{ edu.years }}</li>
        <li><strong>Subject:</strong> {{ edu.subject }} </li>
        <li><strong>Diploma Thesis:</strong> {{ edu.diploma }} </li> 
        <li><strong>Institute:</strong> {{ edu.institute }}</li>
        <li><strong>City:</strong> {{ edu.city }} </li><br>
    {% endfor %}
</ul>

_______________________


<h2>Expirenece</h2>

<ul>
    {% for ex in site.data.experience.experience %}
        <li><strong>Period Time:</strong> {{ ex.years }} </li>
        <li><strong>Job Title:</strong> {{ ex.job }} </li> 
        <li><strong>Employer:</strong> {{ ex.employer }} </li> 
        <li><strong>Company Link:</strong> <a href="http://{{ ex.employerlink }}" target="_blank">{{ ex.employerlink }}</a></li>
        <li><strong>City:</strong> {{ ex.city }}</li><br>
    {% endfor %}
</ul>

_______________________


<h2>Conferences</h2>

<ul>
    {% for conf in site.data.conferences.conferences %}
        <li><strong>Year:</strong> {{ conf.years }}</li> 
        <li><strong>Event name:</strong> {{ conf.event }}</li> 
        <li><strong>City:</strong> {{ conf.city }}</li> <br>
    {% endfor %}
</ul>
_______________________


<h2>Languages</h2>

<ul>
    <li><strong>Greek:</strong> {{ site.data.languages.greek }}</li>
    <li><strong>English:</strong> {{ site.data.languages.english }}</li>
    <li><strong>French:</strong> {{ site.data.languages.french }}</li>
</ul>

