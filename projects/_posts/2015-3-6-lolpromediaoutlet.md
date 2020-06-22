---
layout: post
title: Media Outlet Dashboard
---

![Media Outlet Dashboard]({{ site.baseurl }}/images/lolpromediaoutlet.png "Media Outlet Dashboard")

## Description
 Ruby on Rails web application that displays the latest social media feeds from professional North American League of Legends players. The purpose of this app is to increase fanbase awareness of pro players’ latest news updates.

## Purpose 
To increase fanbase awareness of pro players’ latest news updates

## User Experience
Given any pro player summoner name, LoLProMediaOutlet queries the NALCS database to check if the player exists and is currently playing in the summer split tournament. If player exists, LoLProMediaOutlet will then make API calls to several social media servers, collect relevant information, and organize the data into a single web page.

## Issues
Players without Facebook accounts will display error.
Database is manually created for NALCS summer split. Since new players come and go, this web application will have to be updated often.
Lots of API calls from WEBrick’s single threaded server causes a long web page loading time.

## Future plans
Run a multi-threaded environment to speed up loading time
Automate process to get new players into database
Correctly handle players without all social media profiles
Expand this gaming web application to other industries (i.e. NFL football players)

## Teammates
Matthew Ly, Dhruv Seth
