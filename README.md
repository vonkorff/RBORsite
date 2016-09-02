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
1. Here's number 2! (you should also be bale to type 2. instead of 1. but it could work for both)

Links look like:
[A familiar website](http://www.google.com)
Don't forget the http:// in your links or the site will append the link to the blog URL

![]({{ site.baseurl }}/img/teleport.gif)
Note I used {{ site.baseurl }} in that link instead of the full http://beanandnothingness.com/img/teleport.gif
You should write links that way when linking to anything internal to the website (blog post, code, file, image) so that the links and images work both when working on the site locally and on the live site.
```

Will look like:
### Post non-title header
#### Subheader below that, etc.

* Bullets!
* Bullets bullets!
  * Bullety Bullets
* Etc.

1. Ordered list
1. Here's number 2! (you should also be bale to type 2. instead of 1. but it could work for both)

Links look like:
[A familiar website](http://www.google.com)
Don't forget the http:// in your links or the site will append the link to the blog URL

![]({{ site.baseurl }}/img/teleport.gif)
Note I used {{ site.baseurl }} in that link instead of the full http://beanandnothingness.com/img/teleport.gif
You should write links that way when linking to anything internal to the website (blog post, code, file, image) so that the links and images work both when working on the site locally and on the live site.
