# RBOR website info

Info on why Jekyll is cool, what Jekyll does, and how to set up your own Jekyll site locally and on GitHub Pages is [in my *Programming Historian* lesson](http://programminghistorian.org/lessons/building-static-sites-with-jekyll-github-pages)

**Skip to a section:**

* [Tasks](https://github.com/amandavisconti/RBORsite#tasks)

* [Local work](https://github.com/amandavisconti/RBORsite#local-work)
 
* [Live site](https://github.com/amandavisconti/RBORsite#live-site)

* [Jekyll cheatsheet](https://github.com/amandavisconti/RBORsite#jekyll-cheatsheet)

* [Markdown cheatsheet](https://github.com/amandavisconti/RBORsite#markdown-cheatsheet)

## Tasks
Stuff we need/want to do for the website.

*Sooner:*
- [ ] Create separate dev live site for live testing
- [ ] After domain setup, confirm all URL forms resolve (www/not, end slash/not)
- [ ] Other stuff on my usual web checklist (e.g. SEO, accessibility, loading speed)
- [ ] Blog page => each post in full (or expandable excerpt), rather than list of titles
- [ ] Test site appearance for all possible views:
  - [ ] All OS (mainly for Mac vs PC font-rendering differences)
  - [ ] Browser testing (Firefox, Chrome, Safari; Opera and IE)
  - [ ] Mobile (Android, iOs; phone vert & horizontal views; tablet vert & horiz)
  - [ ] All browser widths/heights
  - [ ] When the window is very wide, the bottom of the banner image on the top is cut off.
- [ ] Remove typing (for now)
- [ ] Change 4 social buttons (under blog posts) to shades of red/dusky purple
- [ ] Get email field => Google Sheet working; share sheet with team
- [ ] Readme info on multiple ways to blog (run Jekyll locally/blog in MD and convert to HTML, blog directly on GitHub.com, blog in HTML)
- [ ] After domain setup, check that Googel Analytics is filling correctly
- [ ] @RBORgames profile customize and set up auto-tweet when a new post hits the repo (= hits the RSS feed); note this immediate on first save of new _posts file
- [ ] Clean up unused code
- [ ] Check if C++ syntax highlighting automatic or requires indvidual encoding

*Later:*
- [ ] Google Analytics custom dashboard to share with team
- [ ] Test webapp icon on mobile homepage
- [ ] Google Analytics: advanced site setup (e.g. tie button clicks/downloads to analytics?)
- [ ] Check the RSS feed is generating correctly
- [ ] Mock up team section (avatars and bios) on dev site
- [ ] Mock up media section (screenshots and video) on dev site

## Local work
```cd``` to your GitHub/RBORsite folder

```bundle exec jekyll serve --watch```

Open localhost:4000 in browser (or http://127.0.0.1:4000)

## Jekyll cheatsheet
To test stuff locally (new plugin, theme, how a new blog post looks):

* See changes on the local site as you make them: While the site is running, after making changes to website files: save the files and refresh the webpage to see the changes—except for the _config.yml file, for which you must stop running the website and restart running the website to see changes.

* Stop local site: Hit control-c on the command line.

## Live site

To move local changes to your live site (new post, settings tweak, etc.):

* Make the desired changes to your website’s local files.

* Open the GitHub Desktop app, make sure your website is chosen in the left sidebar’s list of repositories, and write your commit message summary (and description if desired).

* Click “Commit to gh-pages” in the lower left.

* After the commit has completed, click “Sync” in the upper right.

* Allow 10-90 seconds for your changes to reach GitHub’s web servers, then visit your website and refresh the page to see your changes live. If the change isn't showing up after that, check your email for a failed build message (I will add everyone as repo collaborators and I think that should let you get these notifications?).

## Markdown cheatsheet

You can style just ```code that appears inline``` if you want, or you can...
```
Create a whole block of code
Tooooooo
Just—like—this
```

The following markdown:
```
### Post non-title header
#### Subheader below that, etc.

* Bullets!
* Bullets bullets!
  * Bullety Bullets
* Etc.

1. Ordered list
1. Here's number 2! (you should also be able to type 2. instead of 1. but it could work for both)

For external links:
[A familiar website](http://www.google.com)
Don't forget the http:// in your links or the site will append the link to the blog URL

For external images (not in our website repo):
![](https://www.usa.gov/sites/all/themes/usa/images/Logo_USA.png)

**Important bold information!**
*Italics just get one asterisk on either side.*
For internal links and images (blog post, code, file, etc. that lives in the website directory), you should do something different (which won't work in this README, but will work on your local version of the site and on the Jekyll-generated site):

![]({{ site.baseurl }}/img/teleport.gif)

Note I used {{ site.baseurl }} in that link instead of the full http://beanandnothingness.com/img/teleport.gif
That lets internal links and images work both when working on the site locally and on the live site, instead of breaking on one or the other.
```

### Post non-title header
#### Subheader below that, etc.

* Bullets!
* Bullets bullets!
  * Bullety Bullets
* Etc.

1. Ordered list
1. Here's number 2! (you should also be able to type 2. instead of 1. but it could work for both)

For external links:
[A familiar website](http://www.google.com)

Don't forget the http:// in your links or the site will append the link to the blog URL

For external images (not in our website repo):

![](https://www.usa.gov/sites/all/themes/usa/images/Logo_USA.png)

**Important bold information!**
*Italics just get one asterisk on either side.*
For internal links and images (blog post, code, file, etc. that lives in the website directory), you should do something different (which won't work in this README, but will work on your local version of the site and on the Jekyll-generated site):

![]({{ site.baseurl }}/img/teleport.gif)

Note I used {{ site.baseurl }} in that link instead of the full http://beanandnothingness.com/img/teleport.gif
That lets internal links and images work both when working on the site locally and on the live site, instead of breaking on one or the other.
