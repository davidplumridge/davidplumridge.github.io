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

* Minimalist design
* Low maintenance 
* Simple to make changes / add a new blog post
* Ability to preview changes before they are live
* Low cost

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
  - You can find theme details [here](https://jekyllrb.com/docs/themes/)
  - Override some default styles using this file [here](https://github.com/davidplumridge/davidplumridge.github.io/blob/master/assets/main.scss){:target="_blank"}
  - Changed some default layouts using these files [here](https://github.com/davidplumridge/davidplumridge.github.io/blob/master/_includes) {:target="_blank"}
  - Created some extra pages like this one [here](https://github.com/davidplumridge/davidplumridge.github.io/blob/master/projects.md) {:target="_blank"}
  - Created social data [here](https://github.com/davidplumridge/davidplumridge.github.io/blob/master/_data/socials.yml){:target="_blank"}, a template [here](https://github.com/davidplumridge/davidplumridge.github.io/blob/master/_includes/socials.html){:target="_blank"} and used `include` as shown [here](https://github.com/davidplumridge/davidplumridge.github.io/blob/master/_includes/header.html){:target="_blank"}

### Summary

It's easy to make changes locally, preview them by [starting Jekyll](https://github.com/davidplumridge/davidplumridge.github.io/blob/master/start.sh){:target="_blank"} and push them to GitHub once I am ready. Hopefully this blog / guide helps!

Have a question? Contact me [here](/contact)
