---
title: "How to use the comment function by using Disqus"
date: 2019-04-16 08:26:28
categories: jekyll github pages
tags: github pages jekyll
---

# How to add disqus into my GitHub Pages (with the theme of minimal mistakes)
@(HOWTO)[disqus, jekyll, github.io]

## Sign up to comment on the Disqus

1. click the link to move the disqus :  [link for Disqus](https://disqus.com/profile/signup/)
2. make your own profile.
3. move to the **Admin** and then check **Your Sites** and **Short Name**.
4. If you don't have your **Short Name**, move to the **Add Disqus To Site**.
5. Click the **"GET STARTED"** (on the Bottom) and click **I want to install Disqus on my site**.
6. You can enter your **Short Name** into **Website Name**
7. Select *Category* and *Language*, and then click **Create Site**
8. Select your platform and follows the corresponding instructions.
 
> Short Name이 제일 중요함.
 
## Edit your *_config.yml* as follows:

```yml
comments:
  provider               : "disqus" # false
  disqus:
    shortname            : "your-short-name" # https://help.disqus.com/customer/portal/articles/466208-what-s-a-shortname-
```

* Note that you should replace *your-short-name* with your own **Short Name** of Disqus.

```yml
# Defaults
defaults:
  # _posts
  - scope:
      path: ""
      type: posts
    values:
      layout: single
      author_profile: true
      read_time: true
      comments: true
      share: true
      related: true
```

* Uncomment **comments : true**.
