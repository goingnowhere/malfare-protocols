---
layout: page 
title: Malfare Protocols README
description: Readme for the Malfare Protocols Collection 
---

## Contents
 - [Contributing](#contributing)
 - [How to use me](#how-to-use-me)
 - [Normal people](#im-a-normal-person)
 - [Translators](#im-a-translator)
 - [Geeks](#im-a-geek)
 - [Directory Structure](#directory-structure)
 - [Colophon](#colophon)

## Overview 

This repository contains the protocols used by Malfare at:

 * [Nowhere](http://goingnowhere.org)

It aims to:

 * Make it easier to record/view changes to the protocols;
 * Ease translation burdens; 
 * Allow others to use our protocols; 
 * Share others' work, to reduce reinventing the wheel.

## Contributing 

Amazing! You might find the [Styleguide](styleguide/) useful.

## How to use me 

 - The project has been built to consider multiple languages from the
 start (ish) (hence English-language content living in en/)

 - In case of any dispute though, for Nowhere (at least), the
 **English** language version is **canonical**.

 - Translations are provided to aid those with English as a Second
 Language.

### I'm a normal person

#### (not a geek or a translator)

The protocols and procedures are available through that little menu
thing in the top. Hit it, then "Protocols".

As you might have guessed, this is available at
[malfare.goingnowhere.org](malfare.goingnowhere.org).

### I'm a translator

#### Setup

You might find it useful to install the following free software, if you've
not got them already:

 - [OpenOffice](https://www.openoffice.org/download/)
 - GitHub for [Mac](http://mac.github.com/) or
 [Windows](http://windows.github.com/)
 - A [Text Editor](http://en.wikipedia.org/wiki/Text_editor) you find
 acceptable (some of you may like [Atom](https://atom.io/))

You might find having the [MarkDown
Cheat-Sheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
open in a tab useful, too.

#### Get going
First, a quick crash-course in GitHub, which is where the content lives.

(This has been adapted from [another
introduction](https://github.com/melodykramer/melodykramer.github.io/edit/master/_posts/2015-04-06-learning-github-without-one-line-of-code.md))


 - Create a [GitHub account](https://github.com/)

 - Click on the FORK button in the upper right hand corner of
 [https://github.com/goingnowhere/malfare-protocols](https://github.com/goingnowhere/malfare-protocols).

 - In either a text editor you're comfortable with, or using the web
  interface, make the changes you want, for translations, you'll want
  to
    - create, if needed, a new directory for the language (use the
    two letters column on [language
    codes](http://en.wikipedia.org/wiki/List_of_ISO_639-1_codes));
    - create, within the language directory, a translation for the
    protocol. Also create the 'img' directory there, and a 'xml' directory;
    - translate the 'index.md' file, saving that in the language directory also as 'index.md';
    - translate the 'visio' chart (use OpenOffice Draw for this);
    - export the chart as a PNG image ("File/Export")
    - update the navigation menu file, by creating a new section
    similar to 
        [_includes/navigation.html](https://github.com/goingnowhere/malfare-protocols/blob/gh-pages/_includes/navigation.html#L6-L24)
        (e.g. change ```en/adverse_weather/">Adverse weather```).

 - Submit a pull request &mdash; which is a fancy way of telling us
  you want to make a change &mdash; by clicking on the button marked
 "Create a new branch for this commit and start a pull request."

 - Wait for the changes to be incorporated.

And all of this is public, which is what public media should be (and
why it should all be collected together, by the public and for the
public.)

#### Want more GitHub instructions?
[See this tutorial](https://18f.gsa.gov/2015/03/03/how-to-use-github-and-the-terminal-a-guide/)
which is more advanced than necessary for this project but will be
useful should you decide to use it in the future.

#### Updating translations
See [updating translations](updating-translations.html)

### I'm a geek 

Awesomes!

 - First: check you have a [global
 gitignore](https://help.github.com/articles/ignoring-files/#create-a-global-gitignore)
 to not add OS guff. Check that's sourced, too. Thanks 👍

 - Then fork the repo, clone your copy, and work from there. 

 - In your fork, you might find using git-flow helpful &#8212; we'd
 appreciate it! (especially features)

 - When you're ready, send a PR, and we'll consider merging it :)

We *like* doing things via PRs.

#### Bundle
On the first time run, something like this might be useful:

    cd malfare-protocols
    bundle || gem install bundle && bundle

#### Testing
Running a local copy of the protocols (e.g., if you're updating
things, or translating)

    bundle exec jekyll serve

## Directory structure 

We have protocols in the form of: (*foo* is the individual protocol)

 * Overview document: `foo/index.md` 
 * The drawing ("visio") in LibreOffice Draw format: `foo/xml/shortname.fodg` (XML-y)
 * The diagram exported as image(s): `foo/img/shortname-n.png`

 Use LibreOffice's File/Export option to save the PNG file(s).


## Colophon

 - The protocols have been written and edited by various members of
 the Malfare Team (malfare@goingnowhere.org) over the years. Thank you
 everyone involved.

 - Converting existing MS Word documents to MarkDown was done using
 [Ben Balter's *Word to Markdown*
 repo](https://github.com/benbalter/word-to-markdown).

 - This site uses [Jekyll](https://github.com/jekyll/jekyll)

 - The theme is from [Jekyll themes](http://jekyllthemes.org/)
