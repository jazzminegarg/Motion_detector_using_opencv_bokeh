# Motion-Detection-Using-OpenCV-bokeh
<h2>Idea of Interest : </h2>
<p>You have been approached by a company that is studying human bahavior. Your task is to give them a webcam, that can detect the motion or any movement in front of it. This should return a graph, this graph should contain for how long the human/object was in front of the camera.</p>



 
<h2>Video Capture Windows :</h2>
  
After running the code there 4 new window will appear on screen.
<dl>
<dt>1. Gray Frame:</dt> 
<dd>In Gray frame the image is a bit blur and in grayscale we did so because, In gray pictures there is only one intensity value whereas in RGB(Red, Green and Blue) image thre are three intensity values. So it would be easy to calculate the intensity difference in grayscale.</dd>

<dt>2. Difference Frame:</dt> 
<dd>Difference frame shows the difference of intensities of first frame to the current frame.</dd>

<dt>3. Threshold Frame:</dt> 
<dd>If the intensity difference for a particular pixel is more than 30(in my code) then that pixel will be white and if the difference is less than 30 that pixel will be black.</dd>

<dt>4. Color Frame:</dt> 
<dd>In this frame you can see the color images in color frame along with green contour around the moving objects.</dd>

<h2>Additional Python Libraries Required :</h2>
<ul>
  <li>OpenCV</li>
  
       pip install opencv-python
</ul>
<ul>
 <li>Pandas</li>
  
       pip install pandas
</ul>
<ul>
<li>Bokeh</li>
      
      pip install bokeh
</ul>

<h2>Time Record of Movements :</h2>
  
The Time_of_movements file will be stored in the folder where your code file is stored. This file will be in csv extension. In this file the start time of motion and the end time of motion will be recorded.


<h2>Contour Plotting:</h2>
We make use of the findContours function to define the contour area for our image. And we add in the borders at this stage as well

<h2>Plotting Time Intervals :</h2>

Time Intervals will be plotted using Bokeh Plot.
<h3>Bokeh Library</h3>

Bokeh is an interactive visualization library that targets modern web browsers for presentation. Here, the time intervals are collected by the csv file and then plotted using Bokeh. The green color shows that an object was under motion, time is displayed in milisecond(ms).
<br/>
For bokeh documentation:[Bokeh website](https://docs.bokeh.org/en/latest/)

<h2>Usage :</h2>

<b>The Repository contains 2 python files :</b>
<dl>
  <dt>Motion_detection_using_open_cv.py :</dt>
  <dd>It conatins the code for Motion Detection. By running this file you can detect the motion in front of webcam and can record the start and end time of motion.</dd>
  <dt>Motion_detection_graph.py :</dt>
  <dd>It makes use of Boken Library. By running this file you can plot the time intervals. This file imports the code of motion detection from motion_detector.py, so motion_detector.py needs to be in same directory.</dd>


  
