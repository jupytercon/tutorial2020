# Tutorial Speakers Guide

## General design

Each tutorial consists of several short pre-recorded videos (<30min each), plus written materials to supplement and expand on the presentations, provided as Jupyter notebooks in the tutorial repository. 

During the tutorials week of JupyterCon (5–9 October 2020), pre-recorded videos will air on YouTube Premiere at scheduled times, and tutorial instructors will participate in live discussion with the participants via video conference, also at scheduled times. 
Threaded text chat will be available throughout for all participants and instructors to engage in conversation asynchronously.

JupyterCon will build an online course with the materials provided by the instructors, which will remain available after the conference. 
The instructors' content is always open access and free: videos on the JupyterCon YouTube channel, and notebooks in a GitHub repository (under standard public licenses). 
To access the learning sequences on the course platform, however, participants need to be registered. 

The written materials must be on Jupyter notebooks because the course building process pulls content directly from notebooks in a GitHub repository to display a learning sequence in the online course platform.

## Speaker commitment:
The speakers will be asked to deliver their prepared materials by **September 11, 2020**, for the JupyterCon team to prepare an online course using the materials, on the JupyterCon learning platform. 
The speakers will be asked to participate in “office hours” on a video conference with participants during the tutorials week (5–9 October). Speakers are requested to participate in the chat discussions during the tutorials and conference weeks, as their time permits.

## JupyterCon commitment: 
JupyterCon and NumFOCUS volunteers and staff will build the online courses using instructor-created materials.
All source course material will be publicly available for free (videos on the JupyterCon YouTube channel and Jupyter notebooks on GitHub), but the online courses created in the JupyterCon platform will be accessible to registered participants only. The online course created with the contributed materials will remain after the conference is past. The course platform will embed a discussion forum, using a Mattermost instance provided by NumFOCUS/JupyterCon.

## Infrastructure

JupyterCon will deploy an ecosystem of tools and platforms to provide online learning experiences to all attendees. 
Tutorial instructors will be able to exploit these tools to make their content shine.

### Course platform

We've deployed a full-fledged online course platform, using the Open edX software. 
With speaker-provided materials (video and Jupyter notebooks), JupyterCon volunteers and NumFOCUS staff will build an online course. 
It can include quizzes and auto-graded "homework" exercises, to reinforce the partcipants' learning.

The course platform includes a custom extension that allows creating course content _from any publicly available Jupyter notebook_, using its URL. 
Pulling content from Jupyter notebooks allows us to build a learning sequence from the author-provided content, without duplication.

We also have a custom extension that allows writing exercises for the participants that are tested on-the-fly for correctness. 
This allows creating Jupyter-based "homework" assignments that are auto-graded in the platform.

### JupyterHub/MyBinder

JupyterCon is deploying a dedicated JupyterHub server that all participants will have access to. 
In addition, we've developed integrations so that it will be possible for tutorial attendees to launch a JupyterHub session with the notebooks provided by the instructor, so they can interact with the computable content. 


### Chat server

[Mattermost](https://mattermost.com) is an open-source, self-hosted "Slack alternative." 
We have deployed a Mattermost server, and integrated it to the course platform via single-sign-on, providing a secure environment for all participants to hold text-based conversations throughout the conference.


### Video conferencing

The online course platform also includes a custom plug-in that allows us to schedule video calls using our Webex account. 
Participants will be able to join he call with one click from the course.