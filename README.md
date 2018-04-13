# Scoping Statement: Mixed Reality Demo Bot

## Hackers: 
- Tobiah Zarlez: *SE, CSE US*
- Hun Choi: *PM, CSE APAC*
- Tae Young Kim: *SE, CSE APAC*
- Shahed Chowdhuri: *SE, CSE US*
- Adina Shanholtz: *SE, CSE US*
- Zalina Abdul Halim: *PM, CSE APAC*


## Challenge Statement
Some of SEs/PMs demo MR all the time. Often they only have one headset. Sometimes, it's hard to tell people what to do exactly as the navigate mixed reality for the first time. 

Being able to control a project in real time with just your phone would be very useful for lots of different type of apps. In addtion to all sorts of new cross platform interaction between local and remote users, one MR App to many potential bot sessions.

## How it will work / How it will be built
- Using Unity, create an UWP app that works on either HoloLends and/or immersive headset. 
- UWP App connects to Azure to check "current status" of demo. (For the example, should be which objects and/or scene to load, what colors those objects should be, etc)
- Use a Bot Framework bot to set up a "Host session" and get a "Session ID"
- The "Status" of the demo can be changed in real time by interacting with a Bot Framework bot. (Example command "Change the scene to ___"). From both inside the app, as well as any user interacting with the bot on a chat platform who has the session ID. 

## Solution Architecture (Draft)
![MR Demo Bot Architecture](https://github.com/Ogamja/MRDemoBot/blob/master/images/Architecture.png)

## Leverage Plan
From there, we could implement a simple information based game (like [Keep Talking and Nobody Explodes](https://en.wikipedia.org/wiki/Keep_Talking_and_Nobody_Explodes), or various [Jackbox](https://en.wikipedia.org/wiki/Jackbox_Games) title) and/or generalize the code to engable integration in many different kinds of MR projects
