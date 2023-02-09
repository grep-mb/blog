---
title: "Cool cli commands for macos"
date: 2023-02-09T14:45:06+01:00
draft: false
cover:
    image: ./macos_terminal.jpg
    alt: 'macos terminal' 
    caption: 'macos terminal'
---

# Cool CLI commands for macos
This is a list of amazing cli tools that you can brew or are present by default.

## yank
yank is the yank tool for your cli. To use it simply pipe it after a command and it will allow you to yank a string in the output.
For example, imagine you have a list of docker container running with complex names. Running `docker ps | yank` will allow you to capture the name of the docker container automatically.
```
docker ps | yank
```

## ncdu 
simply brew install ncdu and you will never worry on what exacly to put after `du` command to know all the disk space used.
```
ncdu
```

## imagemagick
You want to convert a .HEIC file into a png one? Simple 
```
brew install imagemagick
magick mogrify -monitor -format png *.HEIC
```

## gnumeric and ssconvert
you want to convert an xlsx file automatically to a csv file. Just run:
```
ssconvert Book1.xlsx newfile.csv
```

## bat
Bat is like cat but with code highlit. Simply brew install it and you'll have it.

## Wifi passowrds
Get access to all your wifi passwords bu simply running:
```
security find-generic-password -wa 'WIFI NAME'
```

Bonus! you can use 
```
security find-generic-password -wa 'WIFI NAME' | yank
```
and you have it copied directly.

## Get a history of all your donwloads 
```
sqlite3 ~/Library/Preferences/com.apple.LaunchServices.QuarantineEventsV* 'select LSQuarantineDataURLString from LSQuarantineEvent'
```
To delete your history, just run the same with delete instead of select

## whois and dig
Just like the website whois, you can query any website to get information about it.
You can also use dig to dig into the dns of a website

## Tracing the path to a website
There is an amazing tool to see the path to a website. Just use:
```
traceroute www.google.com
```

## Toilet !
simply `brew install toilet` and you can everything to an ascii art.
`toilet blog`


