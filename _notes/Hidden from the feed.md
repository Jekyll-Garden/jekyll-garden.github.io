---
title: Hidden from the feed
notetype : unfeed
date : 01-01-2021
---

Tada! This is note is just like any other notes like [[All Markdown Rendered]], but not listed on the feed. Please remember that the intention of unfeed is only to hide from feed, to declutter feed. The note will be in your website, can be hyperlinked and accessed via URL. 

### Obsidian and Handling Private Docs
I use Obsidian to build notes. And the easiest way of keeping private notes from Obsidian away from Github is by using folders and gitignore. Make `_notes` your Obsidian vault, and inside that, create folders, and git ignore the private ones. 

```
Eg
- _notes 
- - Public
- - Private 
- - Journal
- - Essays
```
Then  my .gitignore will contain
```
/_notes/Private
/_notes/Journal
```

so that I won't sharing my private files or daily journal publically! 