# NeuromatchTeachingDemo Instructions
 
As part of your application, we would like you to make a **4 minute video** that showcases your teaching. We don’t want you to spend too long making this video, certainly no longer than 1 hour. You are not competing against others.  We want as many qualified TAs as possible. Instead you are demonstrating to us that you are ready to teach! You can see a sample teaching demo for part of this tutorial [here](https://drive.google.com/file/d/1RJqaPmik0QLt_nrdDNIiTjpbwuqTC8Jr/view?usp=sharing) and for a basic computer science topic [here](https://drive.google.com/file/d/1BsO8Itwfs1J1l7vHcOtjaljrX9hUjqIj/view).  
 
During the Neuromatch Academy summer course you will be leading hands-on tutorials live with a small group of students. At the end of each tutorial period you'll bring your whole group of students back for a short discussion, to review the answers to the tutorial and discuss further.  Of course, in this teaching demo you're making for us there will be no live students.  But we’d like you to review an exercise in this tutorial (a,b,c, or d) as if there were a live audience (though you do not need to interact with this fake audience).  

We essentially want you to: 1) get to know our tutorial, 2) open zoom and hit record and 3) explain one of the exercises as if you were with students who had just finished working that exercise.

In the remainder of this handout, we will provide a lesson plan / tutorial for ridge-regression, as well as detailed instructions about what we would like you to submit. 

## Background

For this tutorial you can assume that your students have just finished hearing a lecture on regularization in regression.  Thus, they’ve been introduced to the use of lasso (L1) and ridge (L2) penalties in regression.  This tutorial is a supplemental activity for that lecture and will be one of the first times that they apply regularization (in the form of ridge-regression) to data.  At this point they’ve also had some experience in the form of lectures and tutorials with linear regression, dimensionality reduction, and should be familiar with what an L1 and L2 norm are.

The learning objectives for this lesson are:

* Define overfitting.
* Describe the motivation for regularization in regression and in other analysis techniques.
* Apply regression with regularization to neural data
* Compare regression analyses with and without regularization

To be clear, we are not asking you to teach all of these concepts or get through all of the exercises in 4 minutes.  It’s nowhere near enough time.  We have provided these to give you context and a sense of what knowledge acquisition you’re trying to support. Focus on explaining just one of the exercises in this tutorial (a,b,c,d). We want you to demonstrate effective teaching, so don’t rush to try to fit everything in.

## Tutorial Description

In this set of exercises we will try to predict the neural activity from videos of animal behavior using ridge-regression.  The data we will use come from a larger dataset published here: https://science.sciencemag.org/content/364/6437/eaav7893.  For the data here, the mouse was not doing a task, and was free to run and whisk and groom as it pleased. In the meantime there was random noise shown on the screen in front of the mouse.

The neural data consists of the activity of excitatory neurons in visual cortex recorded using two-photon calcium imaging. For these exercises it has been pre-processed.  There were originally 5439 neurons, but here we have reduced that to the top 256 principal components sampled at 1Hz.

The behavioral data was recorded for the same period. While the mouse was on the microscope, we captured its face on video and took the top 500 PCs of the motion energy of this video data, sampled at 1Hz. 

This particular group of neurons have been classified as NOT stimulus-selective, so we are interested in understanding what they are doing. The motivation for this regression analysis is to investigate whether the neural activity is explained by mouse behavior.

You can access the jupyter notebook containing the tutorial here: [https://github.com/kbonnen/NeuromatchTeachingDemo](https://github.com/kbonnen/NeuromatchTeachingDemo)

You can run the jupyter notebook any way that you’d like, but we recommend using google colab to run the notebook.  You can open the jupyter notebook manually through [colab](https://colab.research.google.com/github/), or hit this badge to load directly: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/kbonnen/NeuromatchTeachingDemo/blob/master/ridge-regression-tutorial.ipynb)  

## Lesson Plan Example 
You can structure your four minute video any way you like. Here is a sample minute by minute breakdown in case it is useful. 
* < 1 min: Introduce yourself. Give a few sentences about who you are! 
* < 1 min: Give a very brief recap of what regularization is why you might use it. While you should imagine that you are teaching a class of students, don’t feel the need to address them or ask them questions. 
* ~3 mins: Work through part of the tutorial explaining the code and typing in solutions as you go.
 
## How we will evaluate your video 
We are looking for people who are able to communicate well. We’re looking for quality over quantity, so don’t feel pressured to rush through everything. Instead, make sure the content you do get to is clear and easy to follow.  

## Recording the video 
Because we are planning using Zoom during the Neuromatch Academy summer course, we’d like you to record your lesson using Zoom (instructions below).  It should be a “single take” and you shouldn’t do any post-production work on the video.  Don’t fuss about production quality! We are more interested in who you are than on the quality of your audio :-).  

## Uploading the video 
In your round 2 TA application you will need to provide a link to your sample teaching video.  You can do this however you like.  Possible options include but are not limited to sending a link to a private Youtube video, providing a link to a Google Drive file, or providing a link to a dropbox file.  ***Pease make sure the sharing settings are set so that we will be able to access the video if we have the link.***

## Length of the video 
As we mentioned we want the video to be 4 minutes long. You don’t have to conclude nicely -- feel free to cut the video at 4 minutes, even if you aren’t quite done.  **Making mistakes is ok! Point them out and use them as teaching moments.** Do not feel the need to overproduce your video! We are trying to scale here, we hope you understand :-) 

## Zoom Instructions 
* Open Zoom and press “New Meeting” (or “Host a Meeting”). 
* Make sure your microphone is unmuted and your video is on. 
* Zoom has a variety of teaching tools you can take advantage of (though none in particular are required). Press the 
“Share Screen” button and select one of the following: 
* * Choose the window of an IDE you have previously opened if you want to write code 
* * Choose “Whiteboard” if you want to use the built-in whiteboard feature. Feel free to record an actual whiteboard if you have access to that as well, or to not use a whiteboard at all! 
* * Choose “iPhone/iPad” if you’d like to share work on an iPad (having an iPad is not required).
Some tips for sharing your screen: 
To change what screen you’re sharing, hover over the floating green bar with the meeting ID to bring up the menu and hit “New Share”. 
* * You can stop sharing your screen/whiteboard with the red “Stop Share” button. 
* When you’re ready to record, bring up the menu and (if you have screen sharing) press “More” then “Record on this computer” (or just “Record” and then “Record on this computer” if you’re starting without screen sharing). 
* Once you’re finished, hit the square Stop symbol to stop the recording, and then “End Meeting.” Once you’ve ended the meeting, Zoom will save the recording and should automatically open up the folder it was saved to (if not, go to “Documents/Zoom/[insert date of recording + name of Zoom meeting room]”). 
* Upload the mp4 file in that folder (which should be called zoom_0.mp4 or something similar). 
* For more details or troubleshooting, see https://support.zoom.us/hc/en-us/articles/201362473-Local-Recording.​  
 
