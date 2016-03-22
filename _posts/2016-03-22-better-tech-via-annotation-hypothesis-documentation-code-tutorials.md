---
layout: post
title: Better tech via annotation: using Hypothesis to improve your technical documentation, code, and tutorials
permalink: 2016/03/22/better-tech-via-annotation-hypothesis-documentation-code-tutorials
author: 
  twitter: literature_geek
  github: amandavisconti
tags: [digital-humanities, advice-tutorial]
status: publish
type: post
published: true
---

*This piece originally appeared as [a guest post on the Hypothes.is blog](https://hypothes.is/blog/better-tech-via-annotation/).*

Hypothesis makes inline annotation on any web resource possible: a visually small change from comment sections at the end of resources, but a change with a big impact. Whatever your relationship to tech, we've all been here: you're reading through some technical resource (code, documentation, or tutorial) and something doesn't work the way the page says it should. Maybe you want to add details or a better example; maybe you run into an error message or have a questions specific to your circumstances. Maybe you just want to let the author know "you lost me here". 

For tech resources where understanding succeeds or fails line-by-line instead of by paragraph or section, inline annotation—the ability to highlight specific text and discuss it right next to where it occurs—is a vast improvement. Even those resources with comment sections at the bottom have problems specific to that positioning, like low-quality comments stemming from commentators not responding to any actual statement on the page, or having trouble identifying where a tutorial lost them. In this post, I'll cover how a community used Hypothesis to improve a technical resource: how we got our users involved, the types of annotations we observed, and how we're working to automate the workflow from a new annotation to an improved tech resource.

## A community annotates

I'm a member of the digital humanities (DH) community—we're builders, users, teachers, and thinkers around innovative digital tools for literature, history, and other cultural heritage fields (stuff like [3D printing for archaeology](http://scholarslab.org/uncategorized/preserving-reconstructing-teaching-in-3d/), [text analysis of historical memes in newspapers](http://viraltexts.org/), and [interfaces that let readers interpret and discuss challenging novels](http://www.InfiniteUlysses.com)). During the first two weeks in February, [Shawn Graham](http://electricarchaeology.ca/about/) and I used the [#DHannotates](https://twitter.com/hashtag/dhannotates) tag to encourage DHers to switch from passively reading tech resources to actively annotating them via Hypothesis. We focused on one resource: the amazing [Programming Historian site](http://programminghistorian.org/), where novice-friendly lessons on DH tech skills like the following are [authored, edited, and peer-reviewed by community volunteers](http://programminghistorian.org/project-team):

- [Cleaning OCR'd [scanned and digitized] text with regular expressions](https://via.hypothes.is/http://programminghistorian.org/lessons/cleaning-ocrd-text-with-regular-expressions), by Laura Turner O'Hara
- [Getting started with topic modeling and MALLET](https://via.hypothes.is/http://programminghistorian.org/lessons/topic-modeling-and-mallet), by Shawn Graham, Scott Weingart, and Ian Milligan
- [Visualizing historical networks](https://via.hypothes.is/http://programminghistorian.org/lessons/creating-network-diagrams-from-historical-sources), by Marten Düring
- [Corpus analysis with Antconc](https://via.hypothes.is/http://programminghistorian.org/lessons/corpus-analysis-with-antconc), by Heather Froehlich

(Links to all Hypothesis-augmented versions of all the Programming Historian tutorials [can be perused here](https://gist.github.com/amandavisconti/89edd34f998c35705409).)

Maybe you'd like developers to leave comments as they work through your documentation or code. Or maybe you want to support a wider user community. Questions during a tutorial? Ideas for improvements? Get stuck? Want to thank the tutorial's writers and editors? Users can use Hypothesis annotation to add their thoughts and discuss a resource right in its margins.

## Invite your users to interact with your code, documentation, or tutorials

Want to see the kinds of questions and suggestions for improvement Hypothesis enables your users to share? Our [#DHannotates](http://literaturegeek.com/2016/02/02/DHannotates) event drew annotations on tech tutorials such as:

* [Short tips to avoid problems later in the tutorial](https://hypothes.is/a/AVKjiwTOvTW_3w8LyrtI)


* [Further examples of how you can customize a command](https://hypothes.is/a/AVLRKEnQvTW_3w8Ly4k7)
* [On tutorials written from a Mac/Linux perspective, notes on what Windows users should do differently](https://hypothes.is/a/AVKjrSUbvTW_3w8Lyryw)


* [Aggregated reports of error messages encountered while following a tutorial](https://hypothes.is/a/AVLH3b1vvTW_3w8Ly17O) (the more annotations from stymied users, the more an issue might be broadly affecting your community)


* [Request for definitions for abbreviations used in the tutorial](https://hypothes.is/a/AVK7W2hnvTW_3w8Lyx3i)

You can [see a full list here](https://github.com/programminghistorian/jekyll/issues/182#issuecomment-183466725) of the types of feedback [#DHannotates](https://twitter.com/hashtag/dhannotates) garnered on [the Programming Historian tutorials](http://programminghistorian.org/lessons/).

## How do I get my user community interested?

To stir up interest, we invited users of a specific resource ([Programming Historian](http://programminghistorian.org/lessons/)) from a specific user community (digital humanities) using Twitter ([#DHannotates hashtag](https://twitter.com/hashtag/dhannotates)) and the [Digital Humanities Slack](http://tinyurl.com/DHslack). Two tips: 

1. *Keep the initial focus of your encouragement narrowed to a specific webpage or set of related resources.* We'd love the DH community to annotate all our tech resources, but we decided to start with focus on just one website to keep involvement simple.
2. *Encourage people to try annotations **today** by making it clear their thoughts will be read and responded to during the event.*

Why? Users may be more excited to immediately try out a specific experience: 

> *"Come learn markdown basics from [this tutorial](https://via.hypothes.is/http://programminghistorian.org/lessons/getting-started-with-markdown)! And we'll answer any issues you run into if you annotate the lesson this week."*

then to remember there's a new annotation tool to use, the next time they're using your documentation or lessons and run into something they wish they could discuss. Tying annotation into involvement is a great way to attract and include new users in your tech resource's community, too—annotation is a form of contributing that even those with little experience in your programming language can do.

Hypothesis makes getting started annotating easy. The instructions we shared were simple enough to fit in a tweet or two:

1. [*Create a Hypothesis account.*](http://hypothes.is/register)
2. *Prefix the URL of the webpage you want to annotate with https://via.hypothes.is/.* That is, cut and paste that in front of the link to the page you want to annotate.
3. *Annotate!* It's very intuitive: highlight the text you want to talk about using your mouse cursor, and then type in your comment or question. See [Hypothesis' tutorial for student annotators](https://hypothes.is/quick-start-guide-for-students/) for specific steps and pictures that show you everything you can do with annotation.

We also published blog posts on the project for those who wanted [more information](http://literaturegeek.com/2016/02/02/DHannotates) or were interested from the standpoint of [a teacher seeking to support student tech learning in the classroom](http://electricarchaeology.ca/2016/02/02/can-we-fix-it-yes-we-can/).

## If someone annotates, does anyone else know?

For #DHannotates, we encouraged annotation adoption by promising to answer questions during the weeks of the event—or if we couldn't answer a question, we'd at least make sure the issue was recorded where a future volunteer could address it. Tactics for this included creating an issue in the Programming Historian GitHub repo, and trying to find people who can answer questions via Twitter and the [Digital Humanities Slack](http://tinyurl.com/DHslack). 

The inline highlighting made this much simpler than responding to a comments section at the end of each lesson. By focusing on a set of specific experiences (e.g. "Now's the time to learn basic regular expressions and get feedback on any questions as you learn"), potential annotators were encouraged to make the step over the threshold into annotation as a habit, creating a Hypothesis user account and starting to read a new tech lesson.

A great thing about Hypothesis annotations is that annotations are helpful as-is. In cases such as users providing very specific use cases, further information for the curious, or thanks to the authors of a tutorial, some annotations can simply live in the Hypothesis sidebar. For other annotations that suggest a needed change, like reports of error messages or the need to update a tutorial for the latest version of Python, you may want to go further...

## Automate annotations => improvements

Once you start getting annotations on your documentation or tutorials, you'll want a workflow to capture and build on this community input. While there isn't yet an [IFTTT](https://ifttt.com) or [Zapier](https://zapier.com/) Hypothesis channel, you can easily automate managing annotations using a feed. Hypothesis lets you follow RSS or Atom feeds of your annotations in two ways (just switch out the .rss for .atom if using the latter):

1. A stream of all annotations with a given tag (https://hypothes.is/stream.rss?tags=DHannotates)
2. A stream per annotated URL (e.g. https://hypothes.is/stream.rss?uri=http://programminghistorian.org/lessons/intro-to-the-zotero-api)

You can follow the latest annotations through your RSS reader, use a Slack RSS integration to post new annotations to a dedicated Slack channel, or create an issue for each new annotation in your GitHub issue queue to make sure the annotation gets looked at. If you're concerned about cluttering your issues queue, check out the discussion of tactics among the Programming Historian and #DHannotates group happening on [this GitHub issue](https://github.com/programminghistorian/jekyll/issues/182). 

Interested in trying Hypothesis with your own tech resource? Ideas, questions, and suggestions related to using Hypothesis to improve tech resources can be shared using the Hypothesis ([general product](https://groups.google.com/forum/#!forum/hypothesis-forum) and [users forums](https://groups.google.com/forum/#!forum/hypothesis-users)), or by [adding a GitHub issue](https://github.com/hypothesis/h/issues).

*This guest post was written by [Dr. Amanda Visconti](http://www.amandavisconti.com), a UX designer/developer & digital humanities assistant professor at Purdue University Libraries. You can follow her [@Literature_Geek](http://www.twitter.com/literature_geek) or read her posts on digital humanities web development and other DH experimentation at [LiteratureGeek.com](http://www.LiteratureGeek.com).*