#documentation 
# Basics of Obsidian
This is your new *vault*. A *vault* is a folder with your Obsidian files (markdown text files, plug-ins, settings).

Add Files and Folders with the buttons above the file lists (the 2 icons on the left). Sort files and close folders with the other icons.
![[ Pasted image 20240512151617.png| Sidebar File menu icon]]

Make a note of something, [[create a link]], or try [the Importer](https://help.obsidian.md/Plugins/Importer)!

Right-click in the note to get a menu where you can add things like links, paste text, format paragraphs, add graphs / stats, and more.

When you "insert graph" and put what you want in the menu, you can get something like this (Pie chart as example):

```chart
type: pie
labels: [Cool, Cute, Graphs]
series:
  - title: Stats
    data: [1, 2, 1.5]
tension: 0.2
width: 80%
labelColors: true
fill: false
beginAtZero: false
bestFit: false
bestFitTitle: undefined
bestFitNumber: 0
```

Right-click a file or folder name to get options like rename, open in new tab, move file, delete, and so on.

You can collapse the file and folder menu with the menu button (left icon in image below), to have more space to view your notes. Same thing with the right-side menu that show different views and widgets. The other icons are for what you're viewing in the file menu; your folders, search bar, or bookmarked files.
![[Pasted image 20240512151739.png| top bar icons]]

The actions menu icons on the left (default position), might look [something like this](Pasted image 20240512154935.png). But you can change what icons are there by right-clicking the actions menu bar.

You can drag widgets and tabs, into the sidebars. You can pin notes as tabs and use them as additional navigation, even.

And the "command palette" and hotkeys, are your friend. 
![[Pasted image 20240512155120.png | Open Command Palette icon]]
The "command palette" contains basic actions, as well as some of the things you can do that were added by plug-ins. 

The command "templater: replace active templates in a file" or the default hotkeys ALT + R, will activate templater queries like showing what day today is etc. 

You can also insert "templates" into a note through the actions menu or the command palette, which are re-usable notes or parts of notes or snippets, in a designated "templates" folder. Some plug-ins use templates automatically. If you re-use or plan to re-use the same thing over and over again, you can make it into a template.

Templater (queries that transform into relevant information) and Templates (reusable note files and snippets) are related but different things.

[Other information about Templates here](https://help.obsidian.md/Plugins/Templates).


And to add "properties" to a note the easy way, right click the three-dot menu icon to the right, on the note title bar of a note.
![[Pasted image 20240512211702.png|note title bar]]
[and select "add file property"](Pasted image 20240512211543.png) as shown in image link. This adds YAML metadata, that can be used to narrow down the type of note something is, or add tags, whatever.

In the same note title bar, you can toggle the "view" of a note between editing and reading mode by clicking the book / pencil icon.


You can add a note inside another note by linking it as if its an image, as so:
```
![[NoteNameHere]]
```
or specify that you only want to add whats under a header, as so:
```
![[NoteNameHere#HeaderName]]
```

...
Other than all this, Obsidian at its core is a very modular and customizable markdown notes editor with the options to link between notes. 

A lot of things about Obsidian can be changed, and a lot of questions can be searched and found online about it. 

There are also official Obsidian.md forums, different YouTube channels + videos about Obsidian, and official documentation on the Obsidian.md website.

A lot of customization setups and information can be found on GitHub too. 

# This Vault

The [[Home]] note is the "dashboard" and is set to be the note that automatically opens first, in the "homepage" plug-in settings.

The [[Theme Test]] note shows how markdown looks like with the current settings. This vault was installed with "Minimal Theme", and the Plug-in "Minimal Theme Settings".

How to use [multi-columns css snippet here](https://forum.obsidian.md/t/modular-css-layout-snippets-for-wide-views-multi-column-and-gallery/40534), makes it so you can display lists and callouts in multi-columns.

Agenda / Daily Notes is automatically setup through the "Periodic Notes" plug-in (Using a few notes from the "templates" folder as base for what appears in the "agenda" folders like when clicking "open today" in actions menu or other methods). 


> [!NOTE] Notice
> Monthly Note was turned off and taken off for the sake of brevity !


The "Agenda / 4. Calendar" folder is for the "Full Calendar" plug-in, that you can check in the actions menu icon. 

This vault is setup, such that some basic templates for Agenda notes will automatically generate in the homepage when clicking the "daily" and "weekly".
Templater settings has it so when a new note is made, templater queries (the ones with < % ) will automatically process. So things like "yesterday" in the daily note will automatically show the date of back then.

Note: The templates should appear with templater related errors in the queries because they render when made into a proper note.

This vault uses Dataview. 
DataView is an important plug-in and functionality, that lets you collect and view data. This includes things like showing all the files in a folder or that has an attribute or from a certain timeframe, whatever. Some plug-ins require Dataview to function.

Here is an easy way to [generate DataView queries](https://s-blu.github.io/basic-dataview-query-builder/) when you're ab eginner, that you can copy-paste.

For changing how time and dates get displayed in DataView queries or in the daily notes (periodic note plug-in settings) or templates (templater settings), become familiar with the [time formats here](https://momentjs.com/docs/#/displaying/format/).

Check [how to display tasks in Dataview](https://s-blu.github.io/obsidian_dataview_example_vault/20%20Dataview%20Queries/Basic%20Task%20Queries/), the way you want.

Tasks Calendar in the [[Tasks Dashboard]], uses css and js files in the "media files" folder in "tasksCalendar" to be able to operate. But the name of the folder doesn't matter.

Make tasks as a bullet point with brackets [ ].

``` Info
- [ ]
```
And it will become a "task" and give options for scheduled for and deadline, etc.


# Changing Setup and Names

The Folders in this vault that have some "setup" in different settings are the Agenda folder (and the 4 sub-folders), Templates, and Media Files. 

If you wish to change their name or move stuff around, here are the places you have to change as well.

- "Agenda" folder and it's sub-folders, if change:
	- "Periodic Notes" settings. The "Note Folder" location for each periodic note must be updated if changed.
	  ![[Pasted image 20240512164449.png| Note Folder location settings]]
- "Templates" folder, if change:
	- change the settings in "templates" in the "core plugins" section in settings. and in "templater" plugin in "community plugins".
- "Media Files" folder, if change:
	- All media files you copy-paste into this vault, will automatically go into the "Medial Files" folder. You can change this in "Files and Links" in "settings".![[Pasted image 20240512152354.png | Files and Links Settings]]

If you change the vault name from "DollHouse" to something else, change the Agenda links in the "Home" note homepage to match the vault name, so the links still work. 
(like "vault=DollHouse" part, to "vault=Main%20Vault" if change name to "Main Vault". %20 for any spaces in a name.)
![[Pasted image 20240512163548.png| Daily Note link with 'vault = DollHouse' in it]]


You can change around the "Notes" folder and/or make other folders without any issues though.

# Settings

A lot of things can be changed in the "Settings"

Small changes can be done to the theme in the "Minimal Theme Settings" plug-in under the "community plugins" section in "Settings". To change the theme itself go in to the "Settings" - in the "Appearance" section; but when you do, check how it changes your notes and the [[Theme Test]] note.

You can also add CSS snippets for customization in the "CSS Snippets" section.
![[Pasted image 20240512153425.png | Appearance settings in CSS snippets section]]
or in the "Snippets Downloader" plug-in, if the css file keeps getting updated and maintained online (like on github). Snippets Downloader plug-in doesn't exist on the Community plugins place anymore so if you delete it, you'll have to get it from github if you want it again.
























