---
title: 0011 - How I Take Notes
---

I did promise that I'd write about this so here we are. Before we get into the technical details, I think it's a good idea to talk about why I have my notes in a digital format.

There's a short answer to this and a long answer. I'll get the short answer out of the way first:
> It's convenient

Now for the longer answer. It allows me to sift through my notes a lot faster rather than flicking through a notebook and pausing every few seconds to glance at the headings and bullet points. Plus, I can make links between notes which is a game-changer.

Let's compare physical and digital notes purely on their ability to create links. In a physical note, I'd have to write something like "see notes about monetary policy". The problem arises when I have multiple ideas that are similar to one another making it unclear which note about monetary policy I'm referring to. This can be easily overcome by giving each note a unique ID. In a digital note (at least using the software I'm about to mention) I can make a link by typing "\[\[Monetary Policy]]". I still have the problem of which aspect of monetary policy I'm referring to but I could specify by typing "\[\[Monetary Policy#Expansionary]]" which basically means I'm linking to the subheading about expansionary monetary policy.

This can be done with physical notes and a popular method, known as Zettelkasten, originated with physical notes. The creator of this technique, Niklas Luhmann, had a catalogue of over 90,000 notes all written by hand. He used a Unique Identification system (UID) of YYYYMMDDHHII which basically means he zoomed in from the year all the way down to the minute he was writing a specific note. This automatically organises your notes chronologically as well as creating a special ID for each note. He also wrote the topic of each note in addition to the UID so that there were no true duplicates.

Okay now onto the software.

## Software
### [Obsidian](https://obsidian.md)
[[Obsidian]] is my go to note taking tool nowadays. It lets me make links between notes very easily by typing"\[\[" and it'll start autocompleting the link based on what I type. One of the interesting things about it is that it's not a normal text editor. Instead of being something like Word or Google Docs with all the fancy text formatting tools, Obsidian operates on markdown files. This means that your notes will never become outdated due to some technological change and that your notes are stored as plain text.

You can still format your notes but there's a specific syntax you need to follow which took me about 10 minutes to get used to. The only thing you'll need to know to take fully fledged notes is that you use "#" to specify headings and the more of them they are, the smaller the heading ("####" is smaller than "##"). Plus, the versatility of markdown means that it can be used for any purpose. This post you're reading right now was typed using only markdown but it's being rendered perfectly onto your screen.

Unfortunately, Obsidian has only one limitation, but it's intentional: your notes exist as files only on your laptop. This can be worked around though, which brings me nicely tooo

### [GitHub Desktop](https://desktop.github.com/)
For those of you who don't know about GitHub, it's a place where you can store all your code for a project in folders, just like you would on your laptop. Fortunately, it's not limited to just code, it works with any kind of file! This means that we can store all our notes on GitHub which allows us to look at them on any device. Doing this manually would be a complete pain as you'd have to remember which notes you changed after your last backup and then copy the exact changes into your GitHub repository (the online folder with all your files).

This is where GitHub Desktop comes in. It auto detects any changes and all you have to do is confirm which files you want to backup and then send the changes to your repository. Setting up a GitHub repository is a bit more complicated than you'd expect it to be but there's plenty of tutorials for it online.

From your GitHub repo, you can just leave the files there, or you could do something fancier with it like setting it up so you auto-generate a website from your notes (again, this is exactly what I'm doing here).

### [Visual Studio Code](https://code.visualstudio.com/)
This is the optional software, but works fantastically with Obsidian. You see, Obsidian's default appearance is quite boring and you can replace it user-made themes, but if you want to make anything remotely custom, you'll need VSCode. This is because Windows will default to using Notepad to open any text files that are in a strange format, like `.css` and it's just a pain to use. VSCode makes this a lot easier.

Apart from being used for Obsidian styling, VSC is quite versatile and can be used to open any file and I've found it very useful when setting up this site. I made all the changes to the code using VSC alone.

## Conclusion
While I do recommend using the three software I've mentioned above, there also some alternatives. The main one is Roam Research, which has most of the same features as Obsidian but it's a website meaning you don't have to work around Obsidian's local files. The downside? It's quite expensive.

I don't think it's worth the price but it does have a very loyal and helpful following. Apart from cost, there's a few more differences between the two. Obsidian is still technically in its beta phase. Don't let this be a dealbreaker though, when I first started with Obsidian about two months ago, they had just released version 0.7.1, now they're on version 0.8.4. The pace of development is quite impressive, especially when you realise that Obsidian runs only on donations from its community meaning that you can get a version of it for free right now. 