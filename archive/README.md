## Archive

An archived copy of the blog. 

### JavaScript Tip of the Day
_Posted June 05, 2020 by senocular_

Once upon a time I started an AS3 Tip of the Day thread over on the kirupa forums. It helped people to get ramped up with AS3, especially in transition from AS2, and I think people dug it.

Not too long ago, I continued with the tip of the day concept, but this time with JavaScript instead of ActionScript. The result was another kirupa forum: JavaScript Tips of the day!. It's already at 100+ tips, and though new tips are no longer daily, new tips are still frequently coming in. A list of the tips will also be kept on this site: senocular.com: JavaScript Tip of the Day.

### Site Problems
_Posted October 23, 2019 by senocular_

Looks like my host upgraded the backend of my site without letting me know, so things have been down for a few days. I apologize for that. I think I have everything back up and running now.

This does help motivate me in moving some of this content off the site and to some other service where it might be more accessible. I've already done this for the Fireworks extensions... err, at least their source files on github. I'll probably do the same for the rest of the content as well. It's all legacy at this point, sadly, but it can still be helpful.

### The End Has Finally Come for Flash
_Posted July 25, 2017 by senocular_

I still remember my first time learning Flash. It was Flash 4. I believe the 30 day trial had just been released and I was recovering from an operation, bedridden for most of the summer. My only friends were a TV and a computer.

It was on that computer that I discovered flash and started to create animations to help fuel my creative fire. Naturally, the operation had an influence of what I created, as seen with "Suddenly Seeking Surgery" (I had been going by the username BirdE230 at the time).

It wasn't until Flash 5 that I started getting more into ActionScript. I had played around with scripting in Flash 4, but the interface was clunky and overall it felt limiting. Flash 5 greatly opened up the possibilities of what could be done with Flash, and it wasn't long before I was hooked. I had found a passion... one that wasn't trouncing n00bs on StarCraft.

Ultimately my work with Flash (and Fireworks) landed me a job at Adobe - not long after the Macromedia merger. I hadn't been looking for a job; afterall, I was already working at a place I liked and people I loved, but after getting a call one day asking, "Would you like to work at Adobe?" I couldn't say no.

That gave me many years, first supporting, then working with feature and internal systems teams for my passion product, Flash. Though I am no longer working with Flash (still at Adobe though), it still saddens me to see that Adobe is announcing its end of life for Flash. You've treated me well, Flash. I will miss you.

### Fireworks extensions now available on Github
_Posted June 19, 2013 by senocular_

Someone recently directed me to an article from reinegger.net called Adobe Fireworks â€“ a super hero that is hard to kill!. It struck a chord with me, particularly with it's point that Fireworks will continue to live and grow thanks to people who create extensions for it. There was even a link to senocular at the end of the article referencing the many extensions I had posted back in my heyday.

Clicking on the link I came to realize that the last FW extension I posted was in 2008! For that matter, it's been over 2 years (!) since I've really done anything to this site. I never even finished designing it (how typical, right?), and practically forgot how to post anything new here. Nevertheless, having been inspired by the article, I felt like there was yet more I could do for FW. So I decided that I would try to dig up all of the source code for my Fireworks extensions and make them available on Github. And today I did just that. The source files may be incomplete, or slightly outdated, but they're there, and hopefully people can learn from them and use them to help make Fireworks the best tool for the job.

### Flash Platform Versioning
_Posted January 19, 2011 by senocular_

As I mentioned before, I was working on a "tutorial" concerning versioning within the Flash Platform. This is now done enough to share: Flash Platform Versions. It's a little heavy, and more of a brain dump than a tutorial, but hopefully it can shed some light. There is one big takeaway: Nothing is in sync anymore. For example Flash Player is currently at version 10.1. Flash Professional, which used to be in sync with Flash Player, is now at 11. Additionally, though the latest SWF version for Flash Player 10.1 remains 10, for 10.2 it will jump to 11. Confused yet?

### Transform Tool 2 Updates
_Posted December 07, 2010 by senocular_

The new revision of the Transform Tool is still a work in progress. The tool is still in beta but now updates - including new source code - will be made available through a new tutorial page. Feel free to contact me with comments or suggestions.

I can't say that a lot of progress will be quickly, especially since the holidays are arriving, but I wanted to make sure what I had was made available publicly.

### Flash Player 10.2 Beta - More Version Confusion
_Posted December 03, 2010 by senocular_

If you haven't already heard, A beta version of Flash Player 10.2 is now available from Adobe Labs. New features include enhanced video performance, support for IE 9, custom cursors (which I'm most excited about), and enhanced full screen. More information about the release can be found in the labs site and I'm sure in the many other posts around the web that covered this.

What I'd like to address is something else that's new with this release that you might not pick up on at first: the SWF version update. To use new features in 10.2, you have to publish a SWF to target "Flash Player 11", or more accurately, give the SWF a SWF version of 11 (SWF11). This marks the first time that the Target Player Version, or SWF version, no longer matches the Flash Player version of the player with which it is associated. So while the SWF version moves up to 11, Flash Player remains in 10, instead moving up to a new dot-release of 10.2.


### Transform Tool 2 (Beta)
_Posted November 17, 2010 by senocular_

Transform ToolFor a while now, I've been slowly working on a successor to my original ActionScript 3 Transform Tool. The code for that original version was a little hacky and if nothing else, complicated and confusing.

Even though it looks the same, this new version greatly improves on the old. In fact, it was written from the ground up to be more modular, easier to understand and, hopefully, easier to use.

This new version is currently in beta; there are a few minor issues I'd still like to work out, but it is, in its current state, very usable. For now, I will provide it simply as a self-contained download with a basic (Flash CS4) usage sample.

Expect more information and an update sometime in the future (when I have time).

### ActionScript 3.0 Documentation Hole: LoaderInfo SecurityErrorEvent
_Posted November 11, 2010 by senocular_

As mentioned in the recent Security Domains, Application Domains, and More in ActionScript 3.0 tutorial, you have the ability to load SWFs from another domain into your own SWF's security domain when using the Loader class. What wasn't covered was error handling, or specifically, what happens when this fails. In fact, I'll tell you now: a SecurityErrorEvent.SECURITY_ERROR event occurs. This gets dispatched from the Loader's contentLoaderInfo object (a LoaderInfo instance) when a cross-domain policy file does not allow, or does not exist to allow the loading of a cross-domain SWF into the security domain of your SWF. Currently (at least at the time of this writing), however, this is not documented in the AS3 language reference.

So, the next time you add listeners to your LoaderInfo, to be completely covered, make sure you also include one for SecurityErrorEvent.SECURITY_ERROR (though this would only be likely ever to occur if you were messing with security domains which is an unlikely case, nevertheless, you've been warned).

### Part 2: Security Domains, Application Domains, and More in ActionScript 3.0
_Posted October 28, 2010 by senocular_

Part 2 is now up. Whereas part 1 covered security domains, this second, and final portion of the tutorial covers application domains. I don't think I'm quite as comfortable with the explanations in this half of the tutorial, but at least its a good few pages shorter than the security half. Also, when writing the portion covering runtime shared libraries, I didn't realize that as of CS5, Flash Pro also started including some framework additions to make dealing with the process a little easier (namely preloading). With Flash and Flex both doing a lot of the heavy work for you there, some of the lower level details maybe aren't so important anymore? Though, in the end, I guess it doesn't hurt to know a little of what's going on under the hood.
