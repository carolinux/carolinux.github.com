---
layout: project
title: Time Manager
picture: tm-before.png
picture-before-small: tm-before-small.png
picture-after-small: tm-before-small.png
status: finished
role: Core Collaborator
stub: Visualization plugin for geotemporal data 
ranking: 3
---
{% include JB/setup %}
<p> Extending Time Manager has been a project I undertook in my spare time in the period from December 2014 to early 2017. Time Manager is a plugin for the open source GIS software called QGIS that allows the user to animate on the map a spatial dataset that also has a time dimension and then export it as frames. QGIS without the plugin can only render a static map. (At least that was the case until 2018 before QGIS 3.0 came out).</p>
<p> <a href="../../assets/img/project/tm_whoosh.gif">Here is an example gif</a> created with the plugin. There is also <a href="https://www.youtube.com/results?search_query=qgis+time+manager">a lot of cool videos</a> on YouTube.
<h3>Relevant Links</h3>
<ul>
<li><a href="https://github.com/anitagraser/TimeManager">Github repository of the Python code</a></li>
<li><a href="http://www.anitagraser.com">Anita Graser's blog</a> - Anita is the original author/current maintainer and a GIS expert.</li>
<li><a href="https://anitagraser.com/2015/08/10/using-timemanager-for-wms-t-layers/
">Using Time Manager for WMS-T layers</a> - My guest post on Anita's blog announcing the support for one more type of geospatial dataset to animate.</li>
<li><a href="https://qgis2015.wordpress.com/2015/03/11/qgis-timemanager-and-how-the-qgis-community-helped-me/">Blogpost about Time Manager by Søren Zebitz Nielsen</a> - Søren talks about how he used the plugin to produce some materials for his PhD and how he reached out to me to request some additional functionality. This was an interesting collaboration for me as well, to talk with him and figure out what change in the plugin can give him the value he needs to make progress.</li>  
<li><a href="https://www.slideshare.net/anitagraser/time-manager-workshop-at-qgis2015-conference-in-nodebo">Slides from Time Manager workshop</a> - Joint workshop I did with Anita Graser, showcasing some new functionality and then guiding the participants to use it.</li>
</ul>

<h3>Story of my involvement</h3>

<p>I started using the plugin to visualize some data I had and I wanted to make it support more time formats. I went on github to make the changes, and I realized I needed to modify the code in a lot of places to make that change. By the time I had managed to make the change, I had already read and understood half of the codebase.</p><p> The part that I didn't understand was mostly the part of how the UI elements (made in Qt) sent signals and reacted to signals from other elements, but, true to form, I really wanted to. It was night and snowing outside over Christmas holidays when it gently (not unlike a snowflake slowly falling on the ground) clicked with me how these things worked. I proceeded to debug the signal situation and to fix the relevant bugs in the codebase that had made it hard to modify parts of it before. </p>
<p>Another thing that became the responsible thing to do was that, as a new collaborator, whom Anita trusted with write access, I should make sure to preserve the existing functionality when refactoring or making changes. Lots of people were actively using the plugin as well. So I started writing tests.</p>
<p>Story TBC as I build my website more...</p>
