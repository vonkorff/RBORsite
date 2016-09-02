# RBOR website info

## Local work
```cd``` to your GitHub/RBORsite folder

```bundle exec jekyll serve --watch```

Open localhost:4000 in browser

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