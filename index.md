---
layout: page
title: Pick and place with a robot arm!
---

<!--Comment: Above here is the header, we need this to generate the web page-->

<!--Comment: This section is markdown-->

[![logoPicture](images/girlsIntoCodingLogo.jpg)](https://www.girlsintocoding.com/)

A project activity for [Girls Into Coding](https://www.girlsintocoding.com/) using a online version of the free open source [Webots](https://www.cyberbotics.com/) robot simulator.

<!--Comment: End of markdown section-->

<!--Comment: This is html bootstrap-->

<div id="sessionLinkPanel" class="container p-3 my-3 bg-warning">
<h2>Actvity series</h2> 
  <p>This activity session is part of a series on simulating robots, you can see links to all the activities in this series below!</p>
<ul class="list-group">
  <a href="https://meisben.github.io/girlsIntoCoding-robotbenchmark-activity/" target="_blank" class="list-group-item list-group-item-action"><b>Activity session 1:</b> Intro to robot simulation</a>
  <a href="https://meisben.github.io/girlsIntoCoding-robotbenchmark-activity2/" target="_blank" class="list-group-item list-group-item-action"><b>Activity session 2:</b> Pick and place with a robot arm</a>
  <a href="https://meisben.github.io/girlsIntoCoding-robotbenchmark-activity3/" target="_blank" class="list-group-item list-group-item-action"><b>Activity session 3:</b> Giving instructions to a robot using a state machine</a>
</ul>
</div>

<!--Comment: This is the end of html bootstrap-->

<!--Comment: This section is markdown-->

This session is designed to be fun! The idea is that we can follow it together online, but that we can be free to move at our own pace. We're going to be doing some basic python programming in this activity. If you're not too familiar with Python, don't worry, you'll be able to follow along :) ! 

<!--Comment: End of markdown section-->

<!--Comment: This code here is html-->

<!--Comment: This is html paragraph spacing <br>-->
<br>
<br>

<!--Comment: This is html bootstrap-->
<div class="container p-3 my-3 bg-primary">
<h2>Contents</h2>
<ul class="list-group">
  <li class="list-group-item"><a href="#resourcesPanel">Resources</a></li>
  <li class="list-group-item"><a href="#Activity1">Pick and place example code</a></li>
</ul>
</div>

<div id="resourcesPanel" class="container p-3 my-3 bg-info">
<h2>Resources</h2> 
  <p>Here's some resources that may help with the activity</p>
<ul class="list-group">
  <a href="https://www.w3schools.com/python/" target="_blank" class="list-group-item list-group-item-action">Python tutorials at W3 Schools</a>
  <a href="https://www.pythoncheatsheet.org/" target="_blank" class="list-group-item list-group-item-action">Python cheatsheet</a>
  <a href="https://www.cyberbotics.com/doc/reference/index" target="_blank" class="list-group-item list-group-item-action">Webots documentation</a>
  <a href="https://robohub.org/30-women-in-robotics-you-need-to-know-about-2019/" target="_blank" class="list-group-item list-group-item-action">30 women in robotics you need to know about – 2019</a>
</ul>
</div>



<!--Comment: This is the end of html bootstrap-->


<!--Comment: Paragrpah spacing-->
<br>
<br>


<!--Comment: This section is markdown again-->

# Let's get familiar with our robot
---

<!--Comment: End of markdown-->

<!--Comment: Back to html bootstrap -->

<div id="Activity1" class="container p-3 my-3 bg-primary text-primary">
<h2>Activity #1</h2>
</div>

<!--Comment: End of html bootstrap -->


<!--Comment: Back to markdown -->

* We'll be using the [robotbenchmark](https://robotbenchmark.net/) website.
* Click on the **Start** button next to the **Wall Following** activity
* Click on **Start programming this benchmark**
* You should see the scene below


[![logoPicture](images/image1.png)](https://www.girlsintocoding.com/)


First we're going to get familiar with how we control our view of the 3D simulation. We need to find how many ultrasonic sensors there are! Let's control the viewpoint to count how many ultrasonic sensors there are on the robot.

**Use the mouse to move the viewpoint and count the number of sensors**
* **Rotate:** click on a 3D object in the scene with the left mouse button and drag the mouse pointer. The viewpoint will rotate around the object.
* **Translate:** click in the scene with the right mouse button and drag the mouse pointer.
* **Zoom:** click in the 3D scene and roll the mouse wheel. It is also possible to zoom by pressing the mouse wheel and dragging the mouse forward or backwards.
* **Tilt:** press the mouse wheel over the 3D scene and drag the mouse to the left or to the right. Pressing simultaneously the left and right mouse buttons is equivalent to pressing the mouse wheel.


<!--Comment: End of markdown-->

<!--Comment: Back to html bootstrap -->



<div class="container">
  <button type="button" class="btn btn-danger" data-toggle="collapse" data-target="#demo1">Example answer</button>
  <div id="demo1" class="collapse" markdown="1">
  There are 16 ultrasonic sensors, 4 at the front of the robot and 4 at the back!
  </div>
</div>



<!--Comment: End of html bootstrap -->





