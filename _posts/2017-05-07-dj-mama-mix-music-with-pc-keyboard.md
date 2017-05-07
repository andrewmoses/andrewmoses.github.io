---
layout: post
title: "DJ Mama - Mix music with PC keyboard"
date: 2017-05-07
---

Hi! Let me introduce DJ Mama. From it's name you can guess it has something to do with DJaying. Yes, you can play and mix music, change its' tempos and adjust volume levels.

OK, kindly watch the video below to get a glimpse of DJ Mama.

<div class="container">
<iframe src="https://www.youtube.com/embed/Dn0nRWWPRh8" frameborder="0" allowfullscreen class="video"></iframe>
</div>


DJ Mama was purely built using python. It primarily feeds on pygame and vlc.

# Requirements

1. Python 2.7 - [click here](https://www.python.org/download/releases/2.7/) to download
2. Pygame - a python library http://www.pygame.org
3. VLC media player - Get it at http://videolan.org

# Step 1

Download zip or clone the project repo from https://github.com/andrewmoses/DJmama

```
$ git clone https://github.com/andrewmoses/DJmama.git
```

# Step 2

* Install pygame

```
$ apt-get install python-pygame
```

* Change directory into the project's root directory
* Run the app by executing crack.py file.

```
$ python crack.py
```

# Step 3

I have loaded three tracks for you. You can change them as per your desire. Place the tracks which you want to load in the project's root directory. Edit crack.py file and replace the file names with your track names.
```
#first row
p = vlc.MediaPlayer("all.mp3")
#middle row
t = vlc.MediaPlayer("good.mp3")
#lastrow
r = vlc.MediaPlayer("move.mp3")
```

Bring out the DJ in you!
Happy DJaying :)
