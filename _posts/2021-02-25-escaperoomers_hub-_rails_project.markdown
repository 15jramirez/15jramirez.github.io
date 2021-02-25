---
layout: post
title:      "EscapeRoomers Hub- Rails Project"
date:       2021-02-25 23:50:06 +0000
permalink:  escaperoomers_hub-_rails_project
---


I feel into an issue of pacakgemanefest- effort looks like this:
```
Webpacker::Manifest::MissingEntryError in Homepage#welcome
Possible causes:
1. You want to set webpacker.yml value of compile to true for your environment
   unless you are using the `webpack -w` or the webpack-dev-server.
2. webpack has not yet re-run to reflect updates.
3. You have misconfigured Webpacker's config/webpacker.yml file.
4. Your webpack configuration is not creating a manifest.
Your manifest contains:
{
```
After searching and using the recommendations. I found that switching my version of nvm fixed my error. I went one lower, so I ran it 14.5.1. With that new change, I removed my packag.js file along with my yarn file. I ran
```rails webpacker:install```
It fixed the manifest error.


# Onto the project
For my project, I was inspired but this website where people reivew all the escape rooms they have seen. I liked it the escape rooms were on a excel sheet, and not liking to the review itself. So I decied to make an app where users can create a profile, make a review and see the escape rooms available. With the escaperooms, user will be able to see all the reviews associated with that specific escaperoom.


Creating the project was a lititle hard to map out as I had many ideas following through my head. What helped me center was to first map out my routes, and focus one part at a time.

I created user first where I had some trouble with ominauth not working. I could create an accoutn with tumblr, but when it came to logging in with tumblr, I would get an error. I noticed when I would create the account via tumblr, I kept getting ``` rollback:transaction ``` in my database. 
What helped my resovle my issue was running ```user.save! ``` 
Running that bang at the end, rendered a specific error as why my having someone log in via tumblr was not working. So what I did is removed that validation requirement for having a minimun length for password, the login via tumblr started working fine. 

After I moved onto the important chunk of my app, creativing reviews and applying the correct assocations( has_many :though). The diffcult part of creating the project was making sure my params carried out the information to the correct places as well as getting the correct paths, especially when I had dynamic urls. 

# Future Upgrades
I do wish I was able to add in a functionanilty where a user is able to see other profiles even when not logged in. Also, for next time I feel adding a review under an escape room would be a nice thing to add, so a user does not have to go to their view page to make a reivew.

I plan to also make a wish list. With the wish list, a user can add to their profile of escape rooms they wish to see in the future. The user will have the abliy to mark it off as completed once they do the escape rooms, moving it to a section where they can see all the escape rooms completed by them



