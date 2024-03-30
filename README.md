# Overview
This repository contains a simple blog created with Hugo and the Ananke theme. Hugo is a static site generator that allows you to create fast and beautiful websites. Ananke is a modern and minimalist theme that is perfect for blogs.

# Requirements
- Hugo (extended edition, v0.112.0 or later)
- Git
# Setup
Install Hugo:
- Windows: https://gohugo.io/installation/windows/
- Mac: https://gohugo.io/installation/macos/ && brew install hugo
- Install Git: https://git-scm.com/downloads
# Development
Clone the repository: 
```
git clone https://github.com/Onechezzz/hugo-clear-blog.git
```
Navigate to the repository folder: 
```
cd hugo-clear-blog
```
Start Hugo's development server: 
```
hugo server
```
Open your browser and go to http://localhost:1313
# Adding a new post
Create a new Markdown file in the content/posts folder: 
```
hugo new content/posts/my-first-post.md
```
Enter the text of your post in the Markdown file
Save the file
Refresh the page in your browser

# Basic commands
- check the Hugo version
``` 
hugo version 
```
 - start Hugo's development server
``` 
hugo server 
```

- create a new post
``` 
hugo new content/posts/my-first-post.md 
```
Hugo created the file in the ``` content/posts ``` directory. Open the file with your editor.
Add some Markdown to the body of the post, but do not change the draft value.
```
+++
title = 'My First Post'
date = 2024-01-14T07:07:07+01:00
draft = true
+++
## Introduction

This is **bold** text, and this is *emphasized* text.

Visit the [Hugo](https://gohugo.io) website!
```
-Save the file, then start Hugo’s development server to view the site. You can run either of the following commands to include draft content.
```
hugo server --buildDrafts
hugo server -D
```
View your site at the URL displayed in your terminal. Keep the development server running as you continue to add and change content.
When satisfied with your new content, set the front matter draft parameter to false.

# Publish the site
When you publish your site, you typically do not want to include draft, future, or expired content. The command is simple.
- build the Hugo site
``` 
hugo 
```

# Resources
Ananke-theme: https://github.com/theNewDynamic/gohugo-theme-ananke
