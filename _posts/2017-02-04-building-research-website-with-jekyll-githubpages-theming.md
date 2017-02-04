---
layout: post
title: 'Theming Jekyll: Customizing the look of your GitHub Pages-hosted, Jekyll-generated website'
permalink: 2017/02/04/building-research-website-with-jekyll-githubpages-theming
tags: [digital-humanities, scholarly-web-design-and-coding, advice-tutorial]
status: publish
type: post
published: true
---

If you’d like an entirely free, easy-to-maintain, preservation-friendly, secure website over which you have full control—such as a scholarly blog, project website, or online portfolio—using Jekyll and GitHub Pages is a good option. I wrote [a peer-reviewed lesson that will get you started](http://programminghistorian.org/lessons/building-static-sites-with-jekyll-github-pages) over at *[The Programming Historian](http://programminghistorian.org)* (which is a really cool site full of peer-reviewed [lessons](http://programminghistorian.org/lessons) for lots of digital humanities skills and methods). My lesson, like many of the lessons at *[The Programming Historian](http://programminghistorian.org)*, assumes no technical knowledge and is specifically aimed at people who haven't coded or created a website before.

That lesson takes you through publishing a basic website that will look much like this [demo website](https://amandavisconti.github.io/JekyllDemo/). If you enjoy the lesson and want to further customize the look of your website, this blog post will help you do that! (*This post assumes you've read [my lesson](http://programminghistorian.org/lessons/building-static-sites-with-jekyll-github-pages) already.*) Thanks to Daniel Akacki for motivation to write this post!

## Theming

As I mentioned in [my lesson](http://programminghistorian.org/lessons/building-static-sites-with-jekyll-github-pages), "theming" means changing the visual appearance (and sometimes behavior, like adding a comment section or a new menu) of your website. "Styling" is often used to mean changing a site's appearance through CSS (the language that tells a browser how to display things, much like HTML tells a browser how to structure content on a page); "theming" more often means that you're achieving styling through not just changes to existing CSS, but by reusing, customizing, or creating a set of multiple files that change the site's visual appearance.

Before you dive into learning CSS, you can simply reuse (and then tweak or more heavily customize) any of the many existing themes for Jekyll-generated sites. [The Jekyll Themes site](http://jekyllthemes.org/) is a good place to start looking for free themes, and most of the themes have a demo website set up so you can navigate around a site using the theme and really get a feel for how it would look on your website.

[Jekyll moved recently](https://github.com/jekyll/jekyll/issues/4510) from themes that consisted of just adding files to your site folder (some CSS, HTML layouts, images, Javascript, etc.), to themes that you install as Ruby Gems (the way you already had to install Jekyll plugins). This is useful in some ways (e.g. improvements the theme creator makes to their theme can be updated on your website just by your updating the gem), but it can also be confusing for people who aren't familiar with Ruby.

Below, I explain how I took the website you should have at the end of [my lesson](http://programminghistorian.org/lessons/building-static-sites-with-jekyll-github-pages), and changed the site to have a new theme. This isn't the only way to theme, but I think it's currently the easiest way if you're new to web development.

## Switching to the "Hacker" theme

We'll be switching to the "Hacker" theme, for which [you can find the code here](https://github.com/pages-themes/hacker).

![Screenshot of Jekyll-generated GitHub Pages site using the Hacker theme]({{ site.baseurl }}/assets/jekyllhackertheme.png)

I set up a duplicate of 

- the [https://amandavisconti.github.io/JekyllDemo](https://amandavisconti.github.io/JekyllDemo) site I created for my lesson 
- at [https://amandavisconti.github.io/JekyllDemoThemed](https://amandavisconti.github.io/JekyllDemoThemed)

so that we're starting from where [my lesson](http://programminghistorian.org/lessons/building-static-sites-with-jekyll-github-pages) left off.

1. I went to [https://github.com/pages-themes/hacker](https://github.com/pages-themes/hacker), clicked on the green "clone or download" button on the right, and choose to download the files as a ZIP and then unpack the ZIP (usually doubleclicking the ZIP icon will do this).

2. I made a copy of my original site files elsewhere, then deleted everything *inside* my website folder (/JekyllDemoThemed)—but not the folder itself. I then pasted in everything *inside* that unpacked ZIP folder—rather than pasting in the whole folder and its contents.

   We made a copy of your original files so that we can later paste in any posts or pages you want to keep from your original site. 

   *A skippable aside, if you're interested:* Making a copy of your website files before deleting them actually isn't a huge need, since if you've followed my lesson you already have those files committed on GitHub, and can always go back to that or other earlier versions of your site (it's just more hassle, which is why we're making a local copy instead). Also, you *could* keep your original site files as-is and just add in the needed files (and/or code inside files) from the theme, but as someone newer to Jekyll it might be difficult to figure out which files need to be changed and which can stay, which is why we're instead starting from the theme ZIP and importing anything from your original site you want to keep.

3. In the terminal, cd into the website folder. For my file setup, that meant entering `cd /Volumes/Vault101/Documents/GitHubGeneral/JekyllDemoTheme`

4. Enter `script/bootstrap`. Let it finish running.

5. Open your _config.yml file and paste in the following (replacing */JekyllDemoThemed* with the name of your website folder):

   `baseurl: "/JekyllDemoThemed"`

   `url: "localhost:4000"`

6. Paste in the /_posts folder from that copy you made of your old site (if you want the posts from the old site). Paste in the pages from the old site ([about.md](http://about.md/) and [resume.md](http://resume.md/)) if you want them.

7. These pages and posts from the old site reference a layout file that existed for the Minima theme (the theme that your first Jekyll site defaults to), but not for the Hacker theme. So, you need to open each page and change **layout: page **to **layout: default**, and open each post and change **layout: post** to **layout: default**.

8. If you're using the default text in the [about.md](http://about.md/) and [resume.md](http://resume.md/) files I used in my demo site, you need to erase two bits of code from each of these pages. Erase {% raw %}`{% include icon-github.html username="jekyll" %}`{% endraw %} from both pages and erase {% raw %}`{% include icon-github.html username="jekyll" %}`{% endraw %} from both pages. (The Minima theme knew how to handle those calls to include icon images, but the Hacker theme doesn't, so they will make your site not run.)

9. The Hacker theme doesn't automatically add pages to a header menu (like the Minima theme did), but you can still access your pages by typing in their URL, e.g. by visiting [https://amandavisconti.github.io/JekyllDemoThemed/about](https://amandavisconti.github.io/JekyllDemoThemed/about) for the [about.md](http://about.md/) page. You can also add links to these into your theme or the [index.md](http://index.md/) page. I often try to find another theme that has a feature I want—such as a fancy header menu—and then copy and paste pieces of its code into my site by trial and error. [The Jekyll Themes site](http://jekyllthemes.org/) is a great place to look, and trial-and-error copying and pasting from other themes is a great way to get more familiar with how your site works.

That should do it! You can compare your site look and files with mine, if needed:

My new demo site using the Hacker theme: [https://amandavisconti.github.io/JekyllDemoThemed/](https://amandavisconti.github.io/JekyllDemoThemed/)

The repo containing the code that runs the hacker demo site:
[https://github.com/amandavisconti/jekylldemothemed](https://github.com/amandavisconti/jekylldemothemed)