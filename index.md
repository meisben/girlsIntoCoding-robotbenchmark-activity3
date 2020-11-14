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

The idea with this acitivity isn't to become an ACE python programmer in 1 hour, but it's just to get an **appreciation** of programming robots. So that you can use this knowledge for good in the future :)! 

<!--Comment: End of markdown section-->

<!--Comment: This code here is html-->

<!--Comment: This is html paragraph spacing <br>-->
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


![image1](images/image1.png)


First we're going to get familiar with how we control our view of the 3D simulation. We need to find how many ultrasonic sensors there are! Let's control the viewpoint to count how many ultrasonic sensors there are on the robot.

**Use the mouse to move the viewpoint and count the number of sensors**
* **Rotate:** click on a 3D object in the scene with the left mouse button and drag the mouse pointer. The viewpoint will rotate around the object.
* **Translate:** click in the scene with the right mouse button and drag the mouse pointer.
* **Zoom:** click in the 3D scene and roll the mouse wheel. It is also possible to zoom by pressing the mouse wheel and dragging the mouse forward or backwards.
* **Tilt:** press the mouse wheel over the 3D scene and drag the mouse to the left or to the right. Pressing simultaneously the left and right mouse buttons is equivalent to pressing the mouse wheel.


<!--Comment: End of markdown-->

<!--Comment: Back to html bootstrap -->



<div class="container">
  <button type="button" class="btn btn-danger" data-toggle="collapse" data-target="#demo1">Answer</button>
  <div id="demo1" class="collapse" markdown="1">
  There are 16 ultrasonic sensors, 4 at the front of the robot and 4 at the back!
  </div>
</div>

<br>

<!--Comment: End of html bootstrap -->

<!--Comment: This section is markdown again-->

# Let's make our robot move using python functions
---

<!--Comment: End of markdown-->

<!--Comment: Back to html bootstrap -->

<div id="Activity2" class="container p-3 my-3 bg-primary text-primary">
<h2>Activity #2</h2>
</div>

<!--Comment: End of html bootstrap -->

<!--Comment: Back to markdown -->

* We're still going to be using the **Wall Following** activity at the [robotbenchmark](https://robotbenchmark.net/) website. So you can keep this open all the time!
* We're going to get our robot moving!!
* When you're ready to program the robot, right click on it, and select **Edit controller**

![image2](images/image2.png)

* A window will pop up with python code in it! This is how we program our virtual robot.
* Delete all the code in the robot controller window, by hightlighting it all (or pressing **ctrl-A**) and then pressing **delete**
* Copy and paste the code from below into the robot controller window, by hightlighting it all (or pressing **ctrl-A**) then right clicking and pressing **copy**
  
![image3](images/image3.png)

* Start the simulation by following the instrucitons in the image above
* You should see the robot approach the wall, but then reverse quickly when it senses it!
* Have a look at the python functions that are making the robot move in the 'Start of main program' section of the code. We'll discuss these together!


# Let's see how the robot is sensing objects
---

<!--Comment: End of markdown-->

<!--Comment: Back to html bootstrap -->

<div id="Activity3" class="container p-3 my-3 bg-primary text-primary">
<h2>Activity #3</h2>
</div>

<!--Comment: End of html bootstrap -->

<!--Comment: Back to markdown -->

* Let's have a look at how the robot is sensing the wall
* Open up the console by following the instructions in the image below, then run the simulation
![image4](images/image4.png)
* The console is where the robot prints messages to us!
* Let's discuss what it is saying

**Questions**
*Let's answer these questions as a group*
* Can you see the moment at which the robot detects the distance to the wall? 
* How does the robot detect the wall?
* What should the robot do when it detects a wall?


# Let's change the robot's movement behaviour
---

<!--Comment: End of markdown-->

<!--Comment: Back to html bootstrap -->

<div id="Activity4" class="container p-3 my-3 bg-primary text-primary">
<h2>Activity #4</h2>
</div>

<!--Comment: End of html bootstrap -->

<!--Comment: Back to markdown -->

* What would we do if we wanted to change the behaviour of the robot when it reaches the wall? 
* Let's alter the code together to make this happen! Our goal is to make the robot move backwards, but not as far.
* Open the 'controller' (code editor) for the robot
* ![image2](images/image2.png)
* Scroll to the section of the code which looks like this (it should be lines 168-189):

```python
# ~*~*~*~*~*~*~*~*~*~*~*~*~*~*~*~*~*~*
# ~~~~ MAKE YOUR EDITS BELOW HERE ~~~
# ~*~*~*~*~*~*~*~*~*~*~*~*~*~*~*~*~*~*
    
    
print("hello :)")
    
# Move backward 
startMoveBackward(5)
# Keep going until we are 1m away from the wall
while True:
    robot.step(500)
    direction, distance = getClosestObjectToRobot()
    print("direction = {}, distance = {}").format(direction, distance) 
    # If the object is too far, then stop moving backward!
    if distance != None and distance > 1:
        break
    
    
# ~*~*~*~*~*~*~*~*~*~*~*~*~*~*~*~*~*~*
# ~~~~ END OF YOUR CODE EDITS ~~~
# ~*~*~*~*~*~*~*~*~*~*~*~*~*~*~*~*~*~*
```

* Let's discuss this code together.
* How would we change the code so that when the robot changes direction (from fowards to backwards) then it prints our name e.g. "hello there ..."?
* How would we make the robot move backwards less far?
* Take a look at the hint and example answers if you're stuck!

<div class="container">
  <button type="button" class="btn btn-danger" data-toggle="collapse" data-target="#demo2">Hint</button>
  <div id="demo2" class="collapse" markdown="1">
  For printing to the console, try having a look at the code line: print("hello :)")

  For the movement, try having a look at the "if statement"!
  </div>
</div>

<br>

<div class="container">
  <button type="button" class="btn btn-danger" data-toggle="collapse" data-target="#demo3">Example Answer</button>
  <div id="demo3" class="collapse" markdown="1">
  ```python
  # ~*~*~*~*~*~*~*~*~*~*~*~*~*~*~*~*~*~*
  # ~~~~ MAKE YOUR EDITS BELOW HERE ~~~
  # ~*~*~*~*~*~*~*~*~*~*~*~*~*~*~*~*~*~*
      
      
  print("hello there Nikita")
      
  # Move backward 
  startMoveBackward(5)
  # Keep going until we are 1m away from the wall
  while True:
      robot.step(500)
      direction, distance = getClosestObjectToRobot()
      print("direction = {}, distance = {}").format(direction, distance) 
      # If the object is too far, then stop moving backward!
      # We change this value to 0.5 so the robot travels on 0.5m backwards from the wall
      if distance != None and distance > 0.75:
          break
      
      
  # ~*~*~*~*~*~*~*~*~*~*~*~*~*~*~*~*~*~*
  # ~~~~ END OF YOUR CODE EDITS ~~~
  # ~*~*~*~*~*~*~*~*~*~*~*~*~*~*~*~*~*~*
  ```
  </div>
</div>

<br>