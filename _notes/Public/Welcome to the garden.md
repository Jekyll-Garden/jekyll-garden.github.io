---
title : Welcome to the garden
notetype : feed
date : 15-04-2021
---

This is a sample atomic note. As you can see, it appears on the homepage feed. The file is located at `_notes/Public`. The folder `_notes` is my Obsidian Vault. You can add files directly to the `_notes` folder, but I prefer to keep a git-ignored private folder inside my Obsidian to ensure private documents are not accidentally shared. 

For all notes to work properly, we need to have three frontmatter values. (If you check this MD file, you will see them as the first five lines). 
```
title:"Filename" 
notetype: feed | unfeed 
date: DD-MM-YYYY
```
The title should be the same as that for the file name. `notetype` is used to declutter the feed by hiding less relevant, supporting atomic notes from the feed. For example, you can hover on this link, [[The story of a hidden note]], and click to visit the note, but this note is not in the feed, as its notetype is defined as unfeed. And finally, the date is used to sort notes in the latest one first order. (I consider it as the last updated date than created date.)

Btw, backlinks (pages with a link to this page) are listed down. Check that one to see how markdown styles get rendered in this theme.