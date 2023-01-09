---
title: "Research and writing workflow"
author: "Adrian Demleitner"
tags:
	- research basics
	- writing basics
---
# Research and writing workflow
*This is a work in progress and might be heavily expanded upon in the near or far future.*

**Table of Content**
- [Introduction](#Introduction)
- [Overview: Tool and workflow outline](#Overview:%20Tool%20and%20workflow%20outline)
- [Tools](#Tools)
	- [Firefox](#Tools#Firefox)
	- [Zotero](#Tools#Zotero)
	- [Obsidian](#Tools#Obsidian)
	- [pandoc](#Tools#pandoc)
- [Import notes and annotation…](#Import%20notes%20and%20annotation…)
	- […from Zotero](#Import%20notes%20and%20annotation…#…from%20Zotero)
	- […from websites](#Import%20notes%20and%20annotation…#…from%20websites)
- [Writing, thinking](#Writing,%20thinking)
- [Exporting from Obsidian…](#Exporting%20from%20Obsidian…)
	- […to documents](#Exporting%20from%20Obsidian…#…to%20documents)
	- […to websites](#Exporting%20from%20Obsidian…#…to%20websites)


I'm pretty happy with my research and writing setup and I always recommend people to do this or that. So for once, I try to write-up my current workflow and the tools involved. There is only simple rule in place, that pretty much defines what tools I'm using: Own your data!

Data that you are producing needs to be valued as work in the current capitalist environment. So if you didn't get paid for it, you still (have to) own it. It also makes it easier to shift tools and setups if you own your data. Owning data means being freely able to read, move and copy, transform, or delete it.

OK, on to an overview of my tools and their basic functions. The basic functions also outline the general workflow.

## Introduction
In research, you always collect, curate, and consume material such as scientific papers, other textual material, images and videos etc. Guided by your inquiry, research question or project, you produce something new out of the collected and worked on material and your own thoughts. In the last stage, you want to hand your new thing over to other people.

The two main tools in my setup are Obsidian and Zotero. Both are free, but only Zotero is open-source. Both offer paid services that you generally don't need, except if you want to make your life easier or become a power user. Obsidian's raw material are markdown files, which are basically glorified plain text files that you have on your own computer. Zotero works with a database hosted somewhere else, but has superior export abilities. are.na is an image-collection service as a platform. You can use something else here, I just happen to like are.na a lot. hypothes.is is also a service, but free and the platform's code is open-source and has a vibrant community, as well as some great export functionalities. pandoc is open-source and a bit nerdy, and just transforms documents. So, all in all, most of these tools meet my initial criteria of enabling you to own your data.

Let us go over the setups of each tool and then some further setup specialities to glue everything together.

## Overview: Tool and workflow outline
- **Collecting**
	- Firefox - Browse the web, access content
	- Zotero - Collect bookmarks, references, and PDFs
- **Curating**
	- Zotero - Create collections, tag and organize your material
- **Consuming**
	- Zotero - Read, annotate and highlight reading material
	- hypothes.is - Read, annotate and highlighte texts online
- **Writing, Thinking**
	- Obsidian - Make notes, connections and write
	- Zotero - Provides references
- **Publishing**
	- pandoc - Export from Obsidian to documents
	- pancake.sh - Export from Obsidian to websites

## Tools
### Firefox
With Firefox, you'll surf the web and visit websites, platforms with scientific papers, podcasts and video-sites and what not. You can, of course, use any other browser, but why would you do?

- Open an account at [hypothes.is](https://web.hypothes.is/). Then install the [hypothesis bookmarklet](https://web.hypothes.is/help/installing-the-bookmarklet/). This lets you annotate websites.
- Install the [Zotero Connector](https://www.zotero.org/download/) for Firefox. This enables you to safe all kinds of material from the web, from websites, to papers, to videos as a reference in Zotero. I said reference, but we'll talk about that later.

### Zotero
- Download: https://www.zotero.org
- Documentation: https://www.zotero.org/support

In Zotero you collect references to things you want to keep, read, work through, cite in your texts, etc. The references can either just point to another place, like a bookmark, but they can also contain attachments. These attachments are usually either a locally saved snapshot of a website, in case it ever goes offline, but you still need the content, or in most cases, a PDF of the text you want to read.

When you do academic writing, it is best practice to reference your sources that you built upon. As is typical with an academic process, this can be tedious and painful. Zotero tries to take the pain out of it. You can have a folder with all your sources, for example, and with a few clicks have a proper formatted list of sources that you can paste into your document.

- Have the Firefox Zotero Connector extension installed.
- Install the [ZotFile](http://zotfile.com/) plugin installed. It's helps to work with the PDF files in such basic things as automatic renaming, so all your files have the same naming convention (yes, that is important, you don't want to have a mess, do you?).
- Also install the [Better BibTeX](https://retorque.re/zotero-better-bibtex/) plugin. This thingy enables Zotero to produce proper citation keys and make wonderful exports of your collections. That will be important later.

Zotero is also a wonderful tool to read and annotate PDFs. Have a look at the [PDF Reader and Note Editor](https://www.zotero.org/support/pdf_reader) guide. It syncs with mobile, so you could also read on your phone or tablet. I usually make all reading notes in Zotero, even if I don't have a PDF. I simply add the book as a reference (for example via [worldcat.org](https://www.worldcat.org/)) and attach a reading note to it.

### Obsidian
- Download: https://obsidian.md
- Documentation: https://help.obsidian.md/Obsidian/Index

This is where the magic happens. Alternatively, you could have a look at [Zettlr](https://www.zettlr.com/). Compared to Obsidian, it is completely open-source, and the developer is super sympathetic. But it's too sluggish for me and the plugin ecosystem is practically non-existent, making it hard to extend. Obsidian is basically a text-editor with superpowers. One of the basic ideas is, that you can write in something and easily link to another file, over time building up a strong knowledge network.

I use the following plugins for writing:

- [Zotero Integration](https://github.com/mgmeyers/obsidian-zotero-integration): Import and use references that you collected in Zotero as well as automatically import your reading notes from Zotero.
- [Hypothes.is](https://github.com/weichenw/obsidian-hypothesis-plugin): Import your annotations from hypothes.is
- [pandoc](https://github.com/OliverBalfour/obsidian-pandoc): This is a plugin that makes Obsidian able to talk to pandoc. Export your writings, including well formatted references, into documents of your choice including PDFs or Word files
- [Footnotes](https://github.com/MichaBrugger/obsidian-footnotes): Since footnotes in Markdown are a bit tedious to produce, this plugin comes handy, but it messes up a bit.
- [Tidy Footnotes](https://github.com/charliecm/obsidian-tidy-footnotes): Cleans the footnote mess…

All these plugins are installable through the built-in plugin-manager. You see that the goal is actually to get as much material as possible into Obsidian. This is where you spent most of your productive time. Going over your notes and annotations, your resources, piecing them all together and at last, come up with your own material.

How exactly you work in Obsidian is up to you and a whole other rabbit whole I fell in several times…

### pandoc
Just install this one and forget about it. Installation guide can be found here: https://pandoc.org/installing.html.

## Import notes and annotation…
### …from Zotero
#todo

### …from websites
- From hypothes.is, just use the command `Hypothes.is: Sync Highlights`. That will sync all your notes and annotations that you've made online into your Obsidian files. It's buggy at times, but mostly works as intended.

## Writing, thinking
#todo

## Exporting from Obsidian…

### …to documents
First, you need to export a Zotero collection or your whole library (not recommended if you have many items).

- Right-click the collection you want to export and chose **Export Collection…**

![](files/Screenshot%202022-08-19%20at%2020.28.33.png)

The settings you should have ticked are:

- Export Notes (enables you to import your notes and annotation into Obsidian)
- Use Journal Abbreviation (can't remember why, just do it)
- Keep updates (when you add another source to that collection in Zotero it will automatically make a new export)

Use the path to the Zotero BibTeX export file and put it into *Citation database path*. You're free in using whatever you want for *Literature note folder*. That is just the place where the notes end up that you import from Zotero.

As a last step, go into the **pandoc** plugin settings and put the following preferences:

![](files/Screenshot%202022-08-19%20at%2020.31.41.png)

- Export files from HTML or markdown: **Markdown**
- Export folder: **Whatever you want**, I like mine in the same place all the time
- Pandoc path: **Use their guide in the little note to find this value**, you can use mine (`/usr/local/bin/pandoc`) on macOS
- Extra Pandoc arguments: **This is important**

```sh
--bibliography=/Users/adrian/path/to/Export.bib --citeproc --csl=/Users/adrian/path/to/Citation-Style.csl
```

If you don't know what a citation style is yet, just leave out the `--csl=/Users/adrian/path/to/Citation-Style.csl` part. This little piece of information will let pandoc know, that you used references in your text, and tries to replace them accordingly during export.

### …to websites
#todo, but I personally use [pancake.sh](https://codeberg.org/thgie/pancake.sh) for that. It's a bunch of scripts I wrote myself to generate a website from an Obsidian vault.