---
layout: post
title:  "Create your blog on github pages"
date:   2016-09-01 14:22 +0800
categories: github blog jekyll
author: "Ongor"
---

It is easy for us to create a blog with [github pages](https://pages.github.com/) , I would like to show you the building flow here, and we will use [Jekyll](https://jekyllrb.com/) for the blog site.

1. First we should sign up an account on [github](https://github.com/).

2. [Create your github respository](https://github.com/new) for the blog. <br/>*Notics:* the blog repository name must be the same as your username, just like `OngorChow.github.io` , the 'OngorChow' is my github username.

3. Create a directory and clone your blog respository to local. just type the command below in the terminal.<br/>
    <pre>$ mkdir my_blog && cd my_blog<br/>$ git clone https://github.com/username/username.github.io<br/>$ cd username.github.io</pre>
    now, you have got the respository to local. let's go on.
    
4. Install Jekyll and build the site. <br/>
   <pre>
   $ gem install jekyll bundler
   $ jekyll new temp-folder
   $ cd temp-folder
   ~/temp-folder $ bundle install
   ~/temp-folder $ bundle exec jekyll serve
   </pre>
   Now browse to *http://localhost:4000* 
   <br/>
   OK, just stop the local server with `ctrl-c`, and copy all the files in temp-folder to your blog respository directory. (I know this is a stupid way... any suggestion?)
   
5. Go to your respository directory and `$ git add .`, `$ git commit -m 'my blog'`, `$ git push` . 

6. If everything goes well, then you can open your blog on live now: https://[username].github.io

   