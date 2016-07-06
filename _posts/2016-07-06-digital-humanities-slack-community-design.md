---
layout: post
title: The Digital Humanities Slack & Community Design
permalink: 2016/07/06/digital-humanities-slack-community-design
tags: [digital-humanities]
status: publish
type: post
published: true
---

Come join the Digital Humanities Slack, a set of DHy chatrooms! (Visit [tinyurl.com/DHslack](tinyurl.com/DHslack) to join.) **We are open to anyone** with a curiosity about DH and/or related interests (e.g. digital libraries, museums, and archives). Absolutely no expertise needed, and we have several specific chat rooms (called "channels" on Slack) devoted to DH beginners, students, job seekers, and asking all kinds of DHy and digital methods questions. ([Here's a good overview of what Slack is/how to use it](https://get.slack.help/hc/en-us/articles/218080037-Getting-started-for-new-users). I'm happy to answer questions about how to use Slack or what it is via [Twitter](http://www.twitter.com/literature_geek) or [email](mailto:aviscont@purdue.edu), too.)

## DH Slack stats

The DH Slack was created in October 2015 after a suggestion from Ed Summers, and was built by the channel creation and chatting of its members. Nine months later (as of July 6, 2016), we have:

- 700 members (84% of which have used the Slack over the past two weeks)
- 67 "channels" (chat rooms devoted to specific topics)
- 21.3k messages sent
- About 60% of messages are on public channels, with the other 40% being DMs
- 180 files (shared code, documents, screenshots...) have been shared and stored on the Slack
- Matthew Lincoln set up Slack loading screen messages to quote definitions of DH from a variety of practitioners! And when someone types "what is the digital humanities", a bot should respond by pointing you to the 800+ definitions over at [whatisdigitalhumanities.com](http://whatisdigitalhumanities.com).

Channels (chat rooms) are Slack user-created, and the names of channels are represented with a pound sign and no space (#wordlefans). The current channels include:

> **Socializing and community info:** #introductions (share a little about your DH interests and what you do, or let people know about a new channel you created), #conferences, #off-topic (water cooler space for non-DHy chat and GIFs), #jobs, #announcements (events, CFPs, new projects), #hottopic (chat about current general DH issues, like that LARB piece...), #reading (share recent DH and entertainment reading and discuss books), #weeklies (weekly fun themes/survey questions)
>
> **Regional and language channels:** #dh-california, #dh_humanidadesdigital, #dh-tennessee, #dh-bay-area, #dh-baltimore
>
> **Fields:** #libraries, #dh-archives, #museums, #publichistory, #arthistory, #envirohumanities, #mediastudies, #elit, #publishing, #openaccess, #copyright
>
> **Getting started:** #DHanswers (both pulls from the DH Q&A site, and a space for asking new questions), #students (talk about the experience of being a student, doing DH as a student...), #beginners (welcoming space for those just getting started in DH), #tutorialplease (ask for pointers to good tutorials on something you want to learn) and #tutorials (share useful tutorials as you run across them)
>
> **Specific DH methods and practices:** #methodology, #visualization, #data-sharing, #annotation (plus a channel specifically about #hypothes-is annotation), #geospatial, #networks, #coding, #design, #linkeddata, #bots, #crowdsourcing, #gaming, #linux, #machinelearning, #databases, #physcomp, #topicmodel, #bibliography, #textencoding, #texthacking, #textanalysis, #datacuration, #philosophy, #simulation, #music, #sound, #3dscholarship, #codesnippets
>
> **Teaching/learning:** #teachingDH, #digitalpedagogy, #programminghistorian (for discussions around the DH tutorial website)
>
> **And #meta** (to discuss the DH Slack itself)

## Community design decisions

Slack is a comparatively new platform (vs. Twitter), so DHers are still figuring out how it can be useful and how to best run the DH Slack. Anyone can join the DH Slack ([tinyurl.com/DHslack](tinyurl.com/DHslack)) and then visit the #meta channel to participate in decisions about our community design. 

Thank you to everyone who shared thoughts on improving the DH Slack on the Slack, via email, or on Twitter, including DH Slack members Sam Abrams, Kristen Mapes, Matthew Lincoln, Ed Summers, Alan G. Pike, Liz Lorang, Hyperverses, timfinnegan, Jeremy Throne, Brandon Locke, Lincoln Mullen, Brian Croxall, and Micah Vandegrift, and others via Twitter and email.

**tl;dr**: *After community discussion, we're keeping the DH Slack as ephemeral (no longterm archive of all messages) and not allowing people who aren't signed into the Slack to read it. I'd be happy to chat with and amplify the platform of anyone who wants to make a DH Slack alternative that does either/both of these things, and I agree that it would be nice to have a place where Twitter conversations could be comfortably and publicly expanded (e.g. [Hypothes.is](http://Hypothes.is ) annotation?)—it's just that the place to do that right now isn't the DH Slack.*

Below are some of the issues we've been thinking through. I’ve heard reasonable arguments for public readability and/or archiving from people who haven’t been using the Slack. Hearing from non-Slacker users is good, since we want to be careful about decisions that deter others from joining; on the other hand, submitting feedback after using this Slack shows both an understanding of how people have been using it, and buy-in to the outcome of these decisions. (That's what my thinking has been in weighing input from inside and outside the Slack.)

**Code of conduct**. [Our evolving code of conduct lives here](https://github.com/amandavisconti/DHslack/blob/master/CodeOfConduct.md), and Slack members are encouraged to suggest additions or changes via #meta. To summarize, we're dedicated to a harassment-free experience for everyone, with a particular reminder that dismissing or belittling lack of DH, tech, or other experience (e.g. answering questions with links to Let Me Google That For You) is not allowed. We provide a list with specific examples of what constitutes harassment and a statement on handling of "reverse-isms".

**Public reading.** Thanks to Sava Saheli for pointing out that the problem with moving unwieldy Twitter conversations to the DH Slack is that this adds a barrier to public reading not present on Twitter (anyone can sign up for the DH Slack and start using it right away, but you do need to sign up and know how to navigate Slack).

Both Slack and the self-hosted OS Slack alternative Mattermost (that I'll discuss below) don't allow non-signed-in (public) reading. Our workaround would be [Matthew Lincoln's nice solution for exporting Slack messages to a GitHub Pages-hosted Jekyll website](https://github.com/mdlincoln/jekyll-slack). This would require someone to remember to periodically manually export the Slack's messages and upload them to GitHub, and I'm not sure if our 10k message limit would cause a problem (each export would be missing earlier messages, so new exports to GitHub might overwrite old ones, meaning older messages would disappear from the public site--insofar as anything disappears from the web given Internet Archive, screenshots, etc.). One option would be to only export certain channels that are visibly marked as public-readable, rather than exporting the entire DH Slack.

We discussed whether allowing public reading this way would make people more or less comfortable using the DH Slack, reaching out both on the DH Slack to active users, and on Twitter to inactive users and people who haven't joined the DH Slack. I heard more people as neutral or against making any of the DH Slack publicly readable this way, making me think we shouldn’t pursue it for now. A twice-cited reason was that a code of conduct is useful when applied not just to people writing on the Slack, but to people reading it as well; if only signed-in people can read the DH Slack, then we can block anyone who harasses from continuing to do so.

**Message archive.** We're at 21.3k Slack messages, and Slack limits its free plan users to seeing the most recent 10k messages. We discussed whether we should pursue a plan that gives us access to the full archive of messages (or come up with a hack to preserve these on our own, like Matthew Lincoln's solution discussed above). I heard more people who were neutral or against doing this, so we won't do it. One cited reason was that ephemerality was freeing: people tend to use the Slack as a place for informal chat, memes, and gifs as well as scholarship, and knowing you're on the record for whatever you say has a chilling effect on that use. 

**Slack alternative?** Micki Kaufman suggested [Mattermost](https://github.com/mattermost) as a Slack alternative: Mattermost is open-source, not run by a for-profit company, self-hosted, and has a tool to import users from Slack. I think this is a really promising platform, and if we were back in October I'd probably have tried it first before Slack.

For a couple reasons, we're not moving the DH Slack to Mattermost—but anyone is welcomed to set up their own Mattermost install on their servers and create a DH community. I'd happily advertise such as platform on the DH Slack! One reason we're not moving right now is buy-in: people already use Slack for other teams (work, participating in project discussions like [Documenting the Now's awesome chatroom around social media archiving ethics](https://docs.google.com/forms/d/1Wk0JdF2Cty2VHMqpf_QlJXVKQdUtfeeFhaYRben3qaM/viewform)) and can move between those and the DH Slack in the same app, instead of having an additional platform open. We're at 700 members, so although the Mattermost user import tool sounds very useful, we'd need to secure permission and interest from our users to move to that platform, and when this possibility was raised, no one was interested in moving. Someone would also need to provide the web hosting and be willing to maintain and upgrade the installation longterm.

**DH scholarly organization oversight?** We originally approached a DH scholarly organization about sponsoring the DH Slack because doing so would let us use Slack's free non-profit plan, which gives you access to a permanent archive of all your Slack's messages (the free Slack plan we're using now only gives you access to the last 10k messages, although it doesn't delete the hidden messages—you can get access back by upgrading your plan). Just paying for a Slack plan (even with the education discount) is cost-prohibitive as cost is calculated by number of users.

We've decided to no longer seek sponsorship for the Slack non-profit plan, but we're still discussing other ways the DH scholarly organization might sponsor or collaborate with the DH Slack. The way Slack forces one person with super admin privileges to "own" a Slack team is weird and undemocratic in our case, when this Slack exists and thrives because of all its members. I think it would still be worth considering a DH scholarly organization being involved just to help with moderation, and to prevent my using my admin privileges to replace all messages with Hamilton memes.

![Screenshot of Facebook post: "Washington: we are outgunned! outmanned! Hamilton: I have 3 friends if that helps"]({{ site.baseurl }}/assets/hamiltonisawesome.jpg)

Seriously, though, it isn't good for one person to control something with so many members (even assuming my good intentions and trying to mitigate personal biases, I could e.g. be hit by a bus). DH scholarly organization involvement could just mean the organization would let members know about the Slack, but another option could be having a couple people from the organization (possibly from its communications committee) who would explicitly commit to helping with moderation/code of conduct issues if they arise. We might even switch the Slack “owner” to an account that several explicit moderators could use, instead of it just being my personal account, so the community can continue without resting on a single person. 

**Contribute:** I've been trying to synthesize the discussions around these issues, and it's very possible we're missing some issues or that my biases are making me interpret people's responses wrong. Please feel free to tell me so via [Twitter](http://www.twitter.com/literature_geek) or [email](mailto:aviscont@purdue.edu)—your name won't be shared with anyone unless you want it to be. Or if you disagree or think of more reasons why we should reconsider these choices, please let me know! Finally, this isn't a binding decision—we can definitely revisit these questions at any time in the future as issues arise or the Slack evolves.