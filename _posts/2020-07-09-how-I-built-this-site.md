---
layout: post
title:  "How I built this site"
date:   2020-07-09 00:00:00 +1000
comments: true
---

I figured it was about time I join the bandwagon and built my own (minimalist) website where all my projects and interests come together.

I figure a good 'first blog' would be to explain how I built this site. Hopefully this helps other people who are looking to do something similar. 

### My requirements

Here is a simple list of my requirements for a personal website:

* Low cost / free
* Minimalist design
* Low maintenance
* A simple way of adding a new blog post
* Ability to preview changes before they are live

### What I used to make this site

There was no need to re-invent the wheel - there are literally 1000's of blogging platforms out there. 

With that in mind, I went looking for a solution. Here are some of the platforms / tools that considered:

* Wordpress (didn't want the bloat)
* Medium (wanted more control)
* Voice (wanted more control)
* Static site generators (some complex, some looked great)

When I found GitHub pages I didn't see the need to look further. I use GitHub daily and it looks pretty simple to get things set up.

### The stack (summary)

* [namecheap](https://namecheap.com){:target="_blank"} - domain registration (davidplumridge.com)
* [github pages](https://pages.github.com){:target="_blank"} - website hosting
* [Jekyll](https://jekyllrb.com){:target="_blank"} - static site generator
* [Visual Studo](https://visualstudio.microsoft.com){:target="_blank"} - IDE

### Step by step

1. Create the GitHub repository
  - Create a repo called `<your-username>.github.io`
  - Full instructions [here](https://pages.github.com){:target="_blank"}

2. Setup the custom domain `davidplumridge.com`
  - Create a file named CNAME in the repository like this one [here](https://github.com/davidplumridge/davidplumridge.github.io/blob/master/CNAME){:target="_blank"}
  - Setup the DNS records with namecheap. Full instructions [here](https://docs.github.com/en/github/working-with-github-pages/managing-a-custom-domain-for-your-github-pages-site#configuring-an-apex-domain){:target="_blank"}

3. Install Jekyll. I did this by following the 3 commands on their homepage [here](https://jekyllrb.com){:target="_blank"}

4. How I customized the site;
  - You can find themes [here](https://jekyllrb.com/docs/themes/){:target="_blank"}
  - Updated includes [here](https://github.com/davidplumridge/davidplumridge.github.io/blob/master/_includes){:target="_blank"} 
  - Updated layouts [here](https://github.com/davidplumridge/davidplumridge.github.io/blob/master/_layouts){:target="_blank"}
  - Created extra pages like this one [here](https://github.com/davidplumridge/davidplumridge.github.io/blob/master/projects.md){:target="_blank"}

### Some issues that I faced (and the resolutions)

  - Cant find header files for Ruby [here](https://stackoverflow.com/questions/20559255/error-while-installing-json-gem-mkmf-rb-cant-find-header-files-for-ruby){:target="_blank"}
  - Unable to install Jekyll on OSX [here](https://stackoverflow.com/questions/8146249/jekyll-command-not-found){:target="_blank"}
  - Unable to resolve type 'size_t' [here](https://stackoverflow.com/questions/66104935/rails-typeerror-unable-to-resolve-type-size-t-big-sur-m1){:target="_blank"}

### Summary

It's easy to preview changes locally (by starting Jekyll) and then push.