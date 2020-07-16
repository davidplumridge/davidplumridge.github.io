---
layout: post
title: "How I built this site"
date: 2024-06-01 00:00:00 +1000
excerpt: "A short guide on how I made this site"
comments: true
---

A short guide on how I made this minimalist website.

### My requirements

* Minimal cost
* Low maintenance
* A simple blog
* Ability to preview changes on my laptop

### The stack

I explored various blogging platforms but found GitHub Pages to be the best fit due to its simplicity and my daily use of GitHub. Here's the setup I chose:

Namecheap - domain registration (davidplumridge.com)
GitHub Pages - website hosting
Jekyll - static site generator
Visual Studio - IDE

### Step by step

1. Create the GitHub repository
  - Create a repo called `<your-username>.github.io`
  - Full instructions [here](https://pages.github.com){:target="_blank"}

2. Setup the custom domain `davidplumridge.com`
  - Create a file named CNAME in the repository like this one [here](https://github.com/davidplumridge/davidplumridge.github.io/blob/master/CNAME){:target="_blank"}
  - Setup the DNS records with namecheap. Full instructions [here](https://docs.github.com/en/github/working-with-github-pages/managing-a-custom-domain-for-your-github-pages-site#configuring-an-apex-domain){:target="_blank"}

3. Install Jekyll. I did this by following the 3 commands from their homepage [here](https://jekyllrb.com){:target="_blank"}

4. How I customized the site;
  - You can find themes [here](https://jekyllrb.com/docs/themes/){:target="_blank"}
  - Updated includes [here](https://github.com/davidplumridge/davidplumridge.github.io/blob/master/_includes){:target="_blank"} 
  - Updating layouts like this one [here](https://github.com/davidplumridge/davidplumridge.github.io/blob/master/_layouts){:target="_blank"}
  - Adding extra pages like this one [here](https://github.com/davidplumridge/davidplumridge.github.io/blob/master/projects.md){:target="_blank"}

5. Preview your changes locally by starting Jekyll on your laptop before pushing
  - run (mac): bundle exec jekyll serve 

### Some issues that I had to resolve

  - Cant find header files for Ruby [solution here](https://stackoverflow.com/questions/20559255/error-while-installing-json-gem-mkmf-rb-cant-find-header-files-for-ruby){:target="_blank"} (sudo xcode-select --install && sudo xcodebuild -license)
  - Unable to install Jekyll on OSX [solution here](https://stackoverflow.com/questions/8146249/jekyll-command-not-found){:target="_blank"}
  - Unable to resolve type 'size_t' [solution here](https://stackoverflow.com/questions/66104935/rails-typeerror-unable-to-resolve-type-size-t-big-sur-m1){:target="_blank"}
