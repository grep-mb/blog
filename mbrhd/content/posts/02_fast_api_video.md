---
title: "Handling videos with OpenCV and FastAPI"
date: 2023-03-01T11:50:05+01:00
draft: true 
cover:
    image: ./macos_terminal.jpg
    alt: 'macos terminal' 
    caption: 'macos terminal'
tags: ["fastapi", "python", "opencv"]
categories: ["python", "ml", "serving", "fastapi", "opencv"]
---

# Handling a video post call with fastapi 
Few weeks ago I've been asked by a friend to build an API to preocess some video sent by a flutter app. I had to implement a fastapi to capture the video do some processing with opencv and predictions with a ML model then return the processed video.  

I had to use several tricks to handle this. Some of the challenging point where the following one:
* opencv's `VideoReader` method takes as input 




