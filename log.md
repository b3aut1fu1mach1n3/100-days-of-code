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