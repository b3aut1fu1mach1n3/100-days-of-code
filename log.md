# 100 Days Of Code

### Day 1: January 21, 2021

**Today's Progress**:
    Created a bsaic express app that uploades files to sn S3 bucket on AWS.  I worked for more than the hour required, but was able to end the day with a working example.

**Thoughts:** 
    Went pretty well once I decided what I would work on.  Felt overwhelmed trying to pick a direction, and anxious that I would need additional time to learn some new tools.  I decided that I will get going making things using a tech stack that I am already familiar with - MySQL/Mongo, Express, Node, React.  I am very interested in getting good at Gatsby with the ultimate goal of being able to work fast and efficient on potential freelance jobs.

**Link to work:** 
    [Image Uploader in express](https://github.com/b3aut1fu1mach1n3/image-upload)

---
### Day 2: January 22, 2021

**Today's Progress**:
    Created the react app that will be the dev environment for an avatar upload component.  It will allow the user to zoom, pan, and crop the image before uploading the resized image to an s3 bucket.

**Thoughts:** 
    It is not a big strectch to wire up a database to store a username with each avatar for the example app.

**Link to work:** 
    [Image Uploader GUI](https://github.com/b3aut1fu1mach1n3/image-upload-gui)

---
### Day 3: January 23, 2021

**Today's Progress**:
    Worked on the avatar upload component some more. Added a slider to control zoom level.

**Thoughts:** 
    I actually struggled with this for a while. I want to keep this as un-opinionated as possible so I am avoiding component libraries like material or fabric, so there is a bit more to figure out.  I am using a basic html `<input type="range">` element.

**Link to work:** 
    [Image Uploader GUI](https://github.com/b3aut1fu1mach1n3/image-upload-gui)

---
### Day 4: January 24, 2021

**Today's Progress**:
    Took a detour from the avatar component.  Thought it would be cool to set up a bot to tweet each daily log for me whenever I push the daily entry up to github.  Made a couple endpoints, to read the repos commits and the contents of the log file.  Working on parsing the log.

**Thoughts:** 
    Once I get it working I would like to make it a serverless function on azure or aws or something.

**Link to work:** 
    [github-integration](https://github.com/b3aut1fu1mach1n3/github-integration)

---
### Day 5: January 25, 2021

**Today's Progress**:    
    So I got the bot up and working, albeit in a kind of crude form so far.  If everything went to plan, than this was tweeted out programatically to contain the day/hashtag and brief progress blurb from my daily log entry.

**Thoughts:** 
    There is much more work to be done actually, despite the fact that this is a very simple project.  I dont have any validation - particulary to ensure that the message is not longer than twitter's alloted 220 characters.  There are no try/catches or error handling for async operations either.  Oh yea, and I would prefer to ditch the Twit npm package since I only need to make a post.

**Link to work:** 
    [github-integration](https://github.com/b3aut1fu1mach1n3/github-integration)

---

### Day 6: January 26, 2021

**Today's Progress**:
    I cleaned up my twitter bot.  It now runs as a console app in the background (whenever I feel like running it) and pings github every 5min to pull down all the commits on this repo.  I have set it to look for the #100DaysOfCode hashtag in the commit message and compare it to the last recorded one (kept in a text file locally), if it is a new commit then the log entries are pulled down and parsed. The end result is tweeted out by the bot...which you are reading now.

**Thoughts:** 
    Pretty cool little node project.  The twitter bot aspect was dead simple using the Twit library.  I am ready to move on for now, but there is lots of fodder here for future enhancements: 1. remove Twit dependency, I only need the most minimal functionality from it, 2. deploy as a serverless function or github action, it is really just a toy in its current implementation since I have to keep it running locally or just start it when I am going to push to this repo.  It was worth the effort to not have to type the same thing twice and it was a fun mini project.

**Link to work:** 
    [github-integration](https://github.com/b3aut1fu1mach1n3/github-integration)

---

### Day 7: January 27, 2021

**Today's Progress**:
    Returned to the avatar editor react component. I made a reusable slider component and wired it up to the image zoom. 

**Thoughts:** 
    I am really happy with the slider component.  It isn't anything too special, but it is cool to skip the bootstrap/material/fabric/(insert component library here). It has actually inspired me a bit to start a library of extensible components and my own style system.  It would be alot, but I would keep things simple and leverage the great flex/grid api's in modern css.

**Link to work:** 
    [Image Uploader GUI](https://github.com/b3aut1fu1mach1n3/image-upload-gui)

---

### Day 8: January 28, 2021

**Today's Progress**:
    Well, you can't win 'em all. I continued on the avatar editor, but didn't make any progress that I could push. Specifically I am working on grabbing the image from the canvas on clicking save. I have been doing the project in typescript and all functional components thus far, which are not playing nice with react-avatar-editor. I have had to adapt my on solutions from the docs for the image canvas component, and refactor the main component to be class-based instead of functional/using hooks.

**Thoughts:** 
    Pretty much said it all in the progress section.  It wasn't a bad day or anything, I just didn't have that cathartic moment of solving a problem. It was quite a rough evening with my daughter as well - major tantrum that put the whole family on edge.  Alexis and I have been doing a 30-day yoga challenge since January 1st though, and that really helped settle me down.  Put in ,y hour and calling it a night.  I have been spending what might actually be way to much time in our bedroom at my makeshift home office.  8 or 830am to 6pm, then 730 or 8 to 11 or later (just lately).  That is about 13 hours a day in a crappy salvaged office chair in a messy room.  Yikes! night night, be back at it again tomorrow!

**Link to work:** 
    [Image Uploader GUI](https://github.com/b3aut1fu1mach1n3/image-upload-gui)

---

### Day 9: January 29, 2021

**Today's Progress**:
    Yesterday I listened to a SyntaxFM podcast about Deno, and it got me all fired up to give it a shot. Today I read documentation, set up my environment and did some hello-world stuff. Very interesting stuff.

**Thoughts:** 
    Really interested in learning Deno. It provides a runtime for TypeScript and Javascript out of the browser, but apparently browser aps too?!?!

**Link to work:** 
    [Deno Documentation](https://deno.land/manual@v1.7.1/getting_started/setup_your_environment) 

---

### Day 10: January 30, 2021

**Today's Progress**:
    I have two courses in the backlog that I have been struggling to find the time to complete - Master Batsby and Advanced React, both by Wes Bos.  Got going on the Gatsby one today.

**Thoughts:** 
    The original rules state that tutorials don't count, but I am going to do them from time to time.  I simply will never find the time to be able to do both, and I really need some of the info from the course to work on the things that I want to do myself.

**Link to work:** 
    [Master Gatsby Course](https://mastergatsby.com/)

---

### Day 11: January 31, 2021

**Today's Progress**:
    Today I continued with the Gatsby course. I have made it through the basic tooling and setup. We have made a skeleton site with routing and a layout component that wraps each page. Dump pages in a pages folder, make a file called 'gatsby-browser' and add a component that will wrap every page rendered from the pages folder

**Thoughts:** 
    I am liking Gatsby so far. It appears to be very very very developer friendly, especially for a certain subset of sites - static or mostly static sites. I take that to mean sites that have very little or no dynamic content, like a landing page or portfolio, or in this case a pizza shop.  

**Link to work:** 
    [Master Gatsby Course](https://mastergatsby.com/)

---

### Day 12: February 1, 2021

**Today's Progress**:
    Continued on Gatsby course. Today we worked with Styled Components to style the nav and layout, and booted up the Sanity Headless CMS. So far I am impressed.

**Thoughts:** 
    Wow, I can see this stack being very efficient and lucrative for the right target audience. Sanity is pretty badass from what I can tell so far, but I have never worked with one before. I honestly hadn't given CMS much thought, but I see now that there is really no reason to roll-your-own at this point.

**Link to work:** 
    [Master Gatsby Course](https://mastergatsby.com/)

---