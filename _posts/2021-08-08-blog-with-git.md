---
title: "Post: Start Blogging With Markdown and Git"
last_modified_at: 2021-08-08
categories:
  - Tech
tags:
  - Blog
  - Git 
  - Jekyll
  - Minimal Mistakes
  - Ruby 
---
### Intention in times of getting into blogging with Git? 
- Learning this, possibly collaborative (for coding and documentation, for example) tool called Git. 
- Well described process and structure of blogging with Jekyll. No need to dive deep into HTML, CSS, JS. Markdown is what you will need to learn, and it's simple enough. 

## Part 1 
### General setting 
**requires some experimentation** (might be fun) and following the guides you can find online. Jekyll blogging depends on a lot of previous infrastructure. Let's skip the basics necessities of your energy, it relies on the platforms, tools and framework as: Ruby, Jekyll, Git (GitHub as a choice), and so on. Thus basic competency in any or all of this might be of benefit. 

I was exploring Jekill blogging initially with Microsoft toolkit, as my work environment was set to use mostly Microsoft products and support Microsoft clients. That's why I started my exploration with PowerShell and VS Code. 

### The guide that I have explored initially: 
- [Start using Git for PowerShell scripts](https://4bes.nl/2019/06/02/step-by-step-start-using-git-for-powershell/) The path travelled, and support on this way. 
  - Ruby (option with Ruby Installer or with WSL on Windows), Ruby gems
  - Git (version control), 
  - GitHub account (Git provider), 
  - PowerShell (Microsoft scripting language),
  - Jekyll (Static Site generator written in Ruby programming language with Minimal Mistakes theme). 

### other refereces 
~~~
Sean Killeen - building Jekyll blog
~~~

## Part 2
### After you have a grasp on Jekyll, you might choose a theme that is different than a default one. 
I've stopped on a Minimal Mistakes first. 

1. [Blogging with Jekyll using Minimal Mistakes Theme](https://purple.telstra.com.au/blog/opensource-blogging-with-jekyll-github-vscode-part-2)

2. Setting comments and Analytics
[Katerina's website was helpful](https://www.cross-validated.com/Personal-website-with-Minimal-Mistakes-Jekyll-Theme-HOWTO-Part-IV/)

## Part 3
### Useful Git commands for initial set up 
- git init
- git status 
- git remote -v (this command checks established connection to the git repository with HTTPS or SSL) 
- git remote remote origin (removing remote from the git brunch) 
- git clone https://github.com/.../.git (makes a local copy of repository from a Git provider like GitHub) 

git add --all (after you edited, removed or added some files - type this to prepare to commit)
git add . (same as git add --all)
git commit -m 'another commit' (another stage of pushing it all to 'final push' to your remote repository)
git push

git push -u
git pull 
git push -u origin master

### Some cleaning in Git without much explanation 
- git clean -d -i (interactive way)
- git clean -d -n (delete, dry run)

### general command line commands 
dir (same as ls, and get-childitem) 
cd .. (go up in a folder) 

### Here is how to quickly introduce a blog to a tech-savvy person by giving him this tool (GitHub account would be required)
- get Minimal Mistakes starter theme (by M. Rose)
- go live with setting > github pages, choosing a branch 

- _config.yml: exclude from processing (bundle, vendor etc.)
- add .bundle/ and vendor/ to .gitignore 

- _config.yml: author, name and other personalized adjustments 
- add ava pic, post images to assets/images/
- edit some pages and delete others? = ready to sent to a friend for a feedback 
- _config.yml: add analytics 

Adding trackers to "_config.yml":
```Ruby 
analytics:
  provider: "google"
  google:
    tracking_id: "" 
    anonymize_ip: true

bing_site_verification: "" (lengthy string comes there)
```

### Jekyll specific 
```ruby 
bundle exec jekyll serve
bundle update
``` 

bundle update jekyll serve
jekyll --v (checks the version) 

### Leaving the last reference as is, it comes together with Jekyll blogging intro
Check out the [Jekyll docs](https://jekyllrb.com/docs/home) for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo](https://github.com/jekyll/jekyll). 

<meta name="msvalidate.01" content="7A96D455B03667537A649E9E535AC3CF" /> 
