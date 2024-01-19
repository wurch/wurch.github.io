---
layout: post
title: "`brew` only MacOs fresh start"
date: 2023-12-31 12:30:00 -0000
---


`brew` only MacOs fresh start
=========

After having had a few macbooks in the past, some Linux machines and other sorts of devices along my developer life, I always felt unconfortable having to use several different methods to install all the things I need.

During these moments that I was dealing with apt; yum; dnf; .dmg packages; .pkg packages; snap; and FlatApp (for god sake I never understood that), one tool always stood out to me, and that was `brew`.

When reading docs and README's, my eyes would glance at `brew` installation process and it always felt much more straight forward, the packages would be more up do date than in other package managers, and looked like it would just work out of the box.

Then I bought a new macbook.
------------
And decided to make an experiment, I would try to install all the software I needed using just `brew`.

It turns out I got very surprised, and all, I mean **all**, software I primarly needed I was able to install with `brew`. And it was as straightforward as it seemed to be. I know there is criticism on it regarding it's speed, and indeed, speed was not one of the highlights of my experience. That being said, this is a sacrifice I'm willing to make, if I get in return the the practicallity and standardization of it. And being honest, for this use case, of a regular user installing software, speed is absolutely not critical.

Summing up with what I installed
-------------
I separated this session in 3 parts, software used to develop other software, software used to improve my desktop experience, and softwares that I use but that there are a ton of reasons to use their concorrent.


### Develop:
- pyenv
- git
- docker
- visual-studio-code
- devtoys

```bash
brew install pyenv git docker visual-studio-code devtoys
```


Desktop Experience
------------
- neovim
- iterm2
- rectangle
- topnotch

```bash
brew install neovim iterm2 rectangle topnotch
```

Opinionated Software
-----------------
- bitwarden
- brave-browser
- spotify
- notion

```bash
brew install bitwarden brave-browser spotify notion
```


# Conclusion
This article is not supposed to be a master piece, but just a reference to my future self. And as with many things in life, maybe the next time I touch this will be to see how wrong I was about all the things I wrote.