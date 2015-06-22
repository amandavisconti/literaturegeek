---
layout: post
title:  "Accessibility Jottings"
date:   2014-12-03 13:00:00
categories: digital dissertation, accessibility
---
{% include image.html url="/assets/accessibilityjottings.JPG" description="List of accessibility foci on dry-erase board, transcribed below in post text" %}

I wrote [a post about accessibility in terms of community inclusivity]({% post_url 2014-05-27-inclusivityeditioncanon %}) previously

I'll be doing a post later on (probably more than one, actually) about accessibility and universal design for digital editions and other digital humanities platforms—this is really just a list I jotted down tonight to help me remember things as I finish up personal testing of the site and begin alpha testing this week. If you'd like to read more about DH and universal design, check out the recommendations below the list!

There will also be an accessibility statement on the digital edition website, including:
what tests I've performed/features I've designed in particular ways to improve universal design or address specific needs
what things I know are problematic, need a type of testing still, or could otherwise be improved
which of the things in the previous list I could use help or advice on
multiple ways to contact me with requests, observations, recommendations

The accessibility jottings list:
==================

Universal design for:
------

+ text fields
+ filters/sorts
+ dropdowns (single-select, multi-select using ctrl+)
+ jQuery sliders (for number/range selection)
+ checkboxes
+ select all/none
+ autosubmit vs. speed/dexterity, time to decide/commit
+ page HTML structure (e.g. default of "annotator-h1" class problematic?)
	- generate screen reading
	- complexity of page (use library catalogue usability/accessibility testing research)
+ text resizing vs. page resizing (does annotation anchoring break?, collapse sidebars for best fit)
+ "mouse bucket challenge": use site start to finish keyboard-only
moving among devices or between print book and digital site
bookmarking, filter/sort persistence (set in profile, update on reading page), page refresh vs. global filter persistence; for keeping "place" in book, and for saving, revisiting, or sharing viewed page w/same displayed annotations+highlights (POST vs. GET, timestamping vs. sorts broken by new latest annotations)
highlight colors and spectrum (for overlapping highlights)
font type and color; page background color
language translation
mobile, tablet use; slow connections (e.g. drop some database queries for better performance when necessary--maybe allow setting this in use profile?)
touch plugin vs. mobile touch/JS concerns
older browsers
Javascript--in general (jQuery, AJAX)
Reasons for not having JS enabled
reading speeds: need more granular bookmarking than per page, e.g. per line (either requires messy line divving or nicer: annotation type that shows up on use profile and links to page with just "bookmark" annotation-type text highlighted, so you know where to start again)
allow bookmarking of multiple pages (vs. progress bar: people peeking ahead, reading parts offline, jumping around book, losing their place, etc. maybe check for linear completion of chapters, but also give users tracking by total individual pages read or percent w/users allowed to add in pages they read in print book so they get a nice realistic quantifier of how much they've read)
friendly to accidental gestures (e.g. click to change what annotations are shown, NOT hover; page flipping; no infinite scrolls)
"Be careful when implementing functionality that changes areas of the page without refreshing the page, such as AJAX. Screen reader software works by taking a virtual copy of the page, which it then interrogates. If the page changes without a refresh (or some indication that the user should refresh their virtual copy) users may be unaware that content has changed."

Some accessibility reading and tool recommendations off the top of my head
==================
* George Williams' "Disability, Universal Design, and the Digital Humanities" in Debates in the Digital Humanities (free online here: http://dhdebates.gc.cuny.edu/debates/text/44) as well as his Digital Dialogue talk on universal design for the digital humanities (with captions: http://mith.umd.edu/podcasts/george-williams-accessibility-digital-environments-language-law-question-inclusion/)

* Tweets using the #a11y hashtag, as well as the #accessiblefuture (and also #accessiblefu or futures, I think?) tag from recent digital humanities accessibility workshops (http://www.accessiblefuture.org/)

* Look for plugins to increase accessibility on your Wordpress etc. sites to make universal design easier: a plugin to convert Wordpress posts to Braille output (https://wordpress.org/plugins/braille/), the Wordpress Accessibility plugin (https://wordpress.org/plugins/wp-accessibility/)

* Resources and testing tools including the W3C's Designing for Inclusion pages (http://www.w3.org/WAI/users/Overview.html), making CPATCHAs accessible (http://accessibility.psu.edu/captcha), browser plugins (e.g. https://chrome.google.com/webstore/detail/accessibility-developer-t/fpkknkljclfencbdbgkenhalefipecmb?hl=en), thinking about colors (http://www.smashingmagazine.com/2014/10/22/color-contrast-tips-and-tools-for-accessibility/), website evaluators (http://wave.webaim.org/ and http://www.tenon.io/)

And: the Game Accessibility Guidelines are for a different type of digital media, but there's overlap with websites—and reading through these helped me discover some ableist assumptions I'd been making about design (http://gameaccessibilityguidelines.com/full-list)