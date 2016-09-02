# RBOR website info

Info on why Jekyll is cool, what Jekyll does, and how to set up your own Jekyll site locally and on GitHub Pages is [in my *Programming Historian* lesson](http://programminghistorian.org/lessons/building-static-sites-with-jekyll-github-pages)

Local work
Jekyll cheatsheet
Markdown cheatsheet

## Local work
```cd``` to your GitHub/RBORsite folder

```bundle exec jekyll serve --watch```

Open localhost:4000 in browser (or http://127.0.0.1:4000)

## Jekyll cheatsheet
To test stuff locally (new plugin, theme, how a new blog post looks):

* See changes on the local site as you make them: While the site is running, after making changes to website files: save the files and refresh the webpage to see the changes—except for the _config.yml file, for which you must stop running the website and restart running the website to see changes.

* Stop local site: Hit control-c on the command line.

To move local changes to your live site (new post, settings tweak, etc.):

* Make the desired changes to your website’s local files.

* Open the GitHub Desktop app, make sure your website is chosen in the left sidebar’s list of repositories, and write your commit message summary (and description if desired).

* Click “Commit to gh-pages” in the lower left.

* After the commit has completed, click “Sync” in the upper right.

* Allow 10-90 seconds for your changes to reach GitHub’s web servers, then visit your website and refresh the page to see your changes live.

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