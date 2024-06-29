---
layout: post
title: "Code snapshot from NeoVim"
description: "How to create code snapshots from NeoVim using CodeSnap"
date: 2024-06-26 18:08:06 +0200
categories: code
---

## The Struggle

Ever wondered how you could create a right-away elegant code snippet to share on your Linkedin post or with a colleague?

The problem arose when I had to write internal tech blogs, documentation, or post mortems.

I’ve always struggled to create nice snippets to show some good or bad pieces of code without the usual code block and copy-paste.

Right-after seeing lots of posts on Linkedin using those kinds of snippets I started digging around and I have found some managed services.

An example is [Snappify.com](https://snappify.com/) but it was too cumbersome to maintain in the long term, with lots of back and forth to adapt the snippet or make changes.

After a couple of writings using this kind of tool, I gave up and went back to the old code block. approach.
## Plot twist

Being relatively new to NeoVim (1 year to date as main editor of choice after several years of fails at using it) I thought that there were no such automation to create snippets from inside NeoVim.

I couldn’t have been more wrong about it, after looking around for a nvim plugin to create “just screenshots” of the code I’ve discovered the perfection.

[Codesnap.nvim](https://github.com/mistricky/codesnap.nvim) 

With a few minutes, I have installed it on my NeoVim environment and quickly generated a snippet as follows:

![Untitled](/assets/codesnap/plot-twist.png)

This snippet has been created in just two steps:

- Selecting the code you want to print in the snippet
- Launching the command to copy the snippet into the clipboard `:CodeSnap`
    
### How to install

If you are using [Lazy]([https://github.com/folke/lazy.nvim](https://github.com/folke/lazy.nvim)) as package manager you just need to add the plugin to the lazy list

![Untitled](/assets/codesnap/lazy.png)

and if you wish to tweak a bit the configuration, just simple add a file called `codesnap.lua` under the folder `nvim/lua/custom/config` .

![Untitled](/assets/codesnap/plugin-settings.png)

### Worth mentioning feature

- `:CodeSnap` to directly copy the generated snippet into the clipboard for a fast paste
- `:CodeSnapSave` to directly save the picture into the configured folder for later usage

### Installation step-by-step guide

For a complete guide, I will redirect you to the Github repository that is really well documented and easy to follow.

[https://github.com/mistricky/codesnap.nvim](https://github.com/mistricky/codesnap.nvim) 
Kudos to the maintainer, let's star the repository :star:

