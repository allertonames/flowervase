[https://github.com/lifeparticle/Markdown-Cheatsheet]()


> [[Skip to main content](https://discuss.logseq.com/t/my-own-cheatsheet/23795#main-container)

[![Logseq](https://discuss.logseq.com/uploads/default/original/1X/4406ff964c0b1db638f9bd0079998a59f36d3526.png)](https://discuss.logseq.com/)

# [My own Cheatsheet](https://discuss.logseq.com/t/my-own-cheatsheet/23795)

[Customization](https://discuss.logseq.com/c/customization/10)[Look what I built](https://discuss.logseq.com/c/customization/look-what-i-built/11)

[1 vote](https://discuss.logseq.com/t/my-own-cheatsheet/23795)

1

# 

[My own Cheatsheet](https://discuss.logseq.com/t/my-own-cheatsheet/23795)

[Customization](https://discuss.logseq.com/c/customization/10)[Look what I built](https://discuss.logseq.com/c/customization/look-what-i-built/11)

[1 vote](https://discuss.logseq.com/t/my-own-cheatsheet/23795)

[![](https://discuss.logseq.com/user_avatar/discuss.logseq.com/sm26/144/14628_2.png)](https://discuss.logseq.com/u/SM26)

[SM26](https://discuss.logseq.com/u/SM26)

[Dec '23](https://discuss.logseq.com/t/my-own-cheatsheet/23795 "Post date")

Hello folks,

I’ve tried several PKMs but so far Logseq seems to stick the best, the low “friction” it has really works for me.  
One thing I like to make for myself is a cheatsheet that I add as favorite, and I use it (in conjunction with templates) as a reference.

It’s a mixed bags of “(My) best practice”, Plugins & markdown documentations

The outcome looks like this, raw page is below  

[![image](https://discuss.logseq.com/uploads/default/optimized/2X/5/5416b7298eb75aed5ccad66e53a57c5747294f54_2_279x500.png)

](https://discuss.logseq.com/uploads/default/original/2X/5/5416b7298eb75aed5ccad66e53a57c5747294f54.png "image")

Raw file

```rust
icon:: 

- Page properties
	- To set properties for a page, you MUST use the first block
	- properties name must be without spaces. e.g. `Hebrew Name::` is bad, but `Hebrew-name::` is fine
	- `icon::` for setting a page icon
	- `alias::` is a way to call the same thing with different names.
	- `page-type::` to inherit icon e.g. [[locations]] and should be used a general type.
		- e.g. Mcdonalds is `page-type:: [[Locations]]` but it's `type:: [[Restaurant]]`
		- page-type is always pages (with [[]]) while type doesn't have (but still can).
	- `type::` is "like a subset" of `page-type::` it can also be set to a block. and it's "more detailed version of" page-type
	- `tags::` is a way to tag a block/page.
		- should I use `#` with tags? how does this work?
	- you can link property value with ``[[]]``, e.g. `birthday::[[10.06.1995]]`
- Use # for statuses and people
	- `#delayed` tasks
	- `#[[Or Gaist]]`
- TODO:
	- use `/TODO` to make a new task
	- you can add `/scheduled` or `/deadline`
	  :LOGBOOK:
	  CLOCK: [2023-11-17 Fri 20:57:34]--[2023-11-17 Fri 20:57:35] =>  00:00:01
	  CLOCK: [2023-11-17 Fri 20:57:35]
	  :END:
	- Add a progress bar with `{{renderer :todomaster}}` or `/todo master`
		- {{renderer :todomaster}}
- Kanban:
	- `/kanban`
	- [ReadMe](https://github.com/sethyuan/logseq-plugin-kanban-board/blob/master/README.en.md)
- namespaces
	- use `/` at the name of the file to use it as folder structure.
	  e.g. `[[Germany/Berlin]]`
- Syntax examples
	- [Style Guide](https://www.logseqtemplates.com/t/candide/Style%20Guide)
	- ### my_checklist_title
	  * [ ] point 1
	  * [X] point 2 
	  * [ ] point 3
- Icon selector
	- [NerdFonts](https://www.nerdfonts.com/cheat-sheet)
	- 🪟WinKey + .
- Plugins
  lastUpdate:: [[18.12.2023]]
	- Show weekday and week-number
	  id:: logseq-plugin-show-weekday-and-week-number
	  Version:: 1.44.0
	  Description:: Show weekday and week number beside journal titles. etc.. mini-calendar for daily page.
	  Author:: YU000jp
	  PluginID:: logseq-plugin-show-weekday-and-week-number
	- Kanban Board
	  version:: 1.17.10
	  description:: Draggable, editable Kanban view.
	  author:: sethyuan
	  pluginId:: logseq-kanban-board
	- Awesome UI
	  version:: 2.4.0
	  description:: Reworked, simplified, fixed and pumped-up Logseq layout.
	  author:: yoyurec
	  pluginId:: logseq-awesome-ui
	- Logseq Calendars
	  version:: 2.2.2
	  description:: Sync your logseq daily note with your google, icloud or outlook calendar
	  author:: Aryan Sawhney
	  pluginId:: logseq-calendars-plugin
		- [Documentation](https://github.com/sawhney17/logseq-calendars-plugin)
	- Logseq Find and Replace
	  version:: 1.1.1
	  description:: Find and Replace across your entire database
	  author:: Aryan Sawhney
	  pluginId:: logseq-find-and-replace
	- Todo list
	  version:: 1.20.0
	  description:: Show your all TODO items and easy to add new items on your today's journal page
	  author:: ahonn
	  pluginId:: logseq-todo-plugin
	- Journals calendar
	  version:: 0.10.10
	  description:: A simple journals calendar plugin for Logseq.
	  author:: xyhp915
	  pluginId:: logseq-journals-calendar
	- Markdown Table Editor
	  version:: 1.8.0
	  description:: Markdown Table Editor
	  author:: haydenull
	  pluginId:: logseq-markdown-table
	- Copy Code
	  version:: 1.2.0
	  description:: Copy code from code blocks to your clipboard
	  author:: vyleung
	  pluginId:: logseq-copy-code-plugin
	- Bullet Threading
	  version:: 1.1.4
	  description:: Add bullet threading to your active blocks in Logseq.
	  author:: pengx17
	  pluginId:: logseq-bullet-threading
	- Recurrence
	  version:: 1.0.7 
	  description:: This plugin allows you to quickly add recurring blocks based on your desired recurrence. It also allows you to delete inserted recurring blocks as well!
	  author:: hkgnp
	  pluginId:: logseq-recurrence-plugin
	- Ordered Lists
	  version:: 0.6.1
	  description:: Ordered lists, flat or nested, multiple formats ordered lists.
	  author:: sethyuan
	  pluginId:: logseq-ol
	- Awesome Links
	  version:: 1.15.16
	  description:: Favicons for external links, page icons for internal
	  author:: yoyurec
	  pluginId:: logseq-awesome-links
	- ToDo Master
	  version:: 1.10.3
	  description:: Render a progress bar to gether the overall progress of the current block or page.
	  author:: pengx17
	  pluginId:: logseq-todo-master
	- Tabs
	  version:: 1.19.3
	  description:: Open pages or blocks in tabs like working in the browser
	  author:: pengx17
	  pluginId:: logseq-tabs
	- Tags
	  version:: 0.1.2
	  description:: A plugin that lets you find and search all of your tags.
	  author:: Gidong Kwon
	  pluginId:: logseq-tags
	- Tabler picker
	  version:: 1.4.0
	  description:: Tabler icon picker plugin for Logseq
	  author:: yoyurec
	  pluginId:: logseq-tabler-picker
	- Habit Tracker
	  version:: 0.4.3
	  description:: Track habits on daily journal pages.
	  author:: c6p
	  pluginId:: logseq-habit-tracker
	- SmartBlocks
	  version:: 3.51
	  description:: A port of the roam SmartBlocks extension with a dash of Notion
	  author:: Aryan Sawhney
	  pluginId:: logseq-smartblocks
		- [Documentation](https://github.com/sawhney17/logseq-smartblocks)
		- [Youtube](https://www.youtube.com/watch?v=55s-K1uAUc0)
	- Awesome Content
	  version:: 1.2.1
	  description:: Enhanced content blocks (tasks, quotes, flashcards, headers, queries, diagrams, etc...)
	  author:: yoyurec
	  pluginId:: logseq-awesome-content
	- Flow Nord theme
	  version:: 0.10.7
	  description:: A minimalist theme that focuses on a clean and sleek interface with various color palette options.
	  author:: nmartin84 and henices
	  pluginId:: logseq-flow-nord-theme```
```

Any feedback would be much appriciated.

- #### created
    
    ![](https://discuss.logseq.com/user_avatar/discuss.logseq.com/sm26/72/14628_2.png "SM26")Dec '23
    
- [
    
    #### last reply
    
    ](https://discuss.logseq.com/t/my-own-cheatsheet/23795/2)
    
    [](https://discuss.logseq.com/t/my-own-cheatsheet/23795/2)![](https://discuss.logseq.com/letter_avatar_proxy/v4/letter/r/278dde/72.png "ruin")Dec '23
    
- 1
    
    #### reply
    

[![](https://discuss.logseq.com/letter_avatar_proxy/v4/letter/r/278dde/144.png)](https://discuss.logseq.com/u/ruin)

[ruin](https://discuss.logseq.com/u/ruin)

[Dec '23](https://discuss.logseq.com/t/my-own-cheatsheet/23795/2 "Post date")

I made one as well and reference it fairly often, less so over time as more things become intuitive. I use the same principle as I do for studying for school though, which is that a cheat sheet should not have things you know on it. Stuff like /TODO or icon:: is very intuitive and easy to remember, so if you’re not looking at the cheat sheet when you do those things, don’t put them on it. Keep it to the stuff that you always find yourself pondering, “ugh, how does that work again?” For me, that was mostly query syntax and hot key shortcuts. Once something is intuitive, I remove it from my cheat sheet. The less stuff on it, the easier it is to find what you need, minimizing time wasted scrolling past stuff you know.

Similarly, if you want keep everything, it might help to add some sub-headers and order the sections & content in sections by what you reference most often, so things you look up a lot are top of the list and stuff you don’t need reference for is near the bottom.

For the question about tags, what I’ve seen most often is using brackets for in-line writing and hashtag for more traditional tagging. For example:

[![IMG_3154](https://discuss.logseq.com/uploads/default/optimized/2X/3/354cd6d42cab80ebd01069fbd9f14bc488695f4a_2_690x139.jpeg)

](https://discuss.logseq.com/uploads/default/original/2X/3/354cd6d42cab80ebd01069fbd9f14bc488695f4a.jpeg "IMG_3154")

Body modification is in brackets because it naturally fit in the sentence, but I had some other pages I wanted this article to be linked for reference, so tossed on some tags. Basically, the hashtag here is the equivalent of ‘this is also related to’. I also have a few utility tags (#to-read, #to-watch, etc.) that I only ever use as tags because the page itself isn’t a topic, it’s just a way of aggregating links. In the end, it’s a stylistic choice, so go with what feels intuitive to you.

### New & Unread Topics

|   |
|---|
|[![](https://discuss.logseq.com/user_avatar/discuss.logseq.com/daniele/144/720_2.png "Daniele")](https://discuss.logseq.com/t/how-to-open-any-file-in-the-mobile-app/24864/1)<br><br>[How to open any file in the mobile app](https://discuss.logseq.com/t/how-to-open-any-file-in-the-mobile-app/24864)|

|   |
|---|
|[Look what I built](https://discuss.logseq.com/c/customization/look-what-i-built/11)<br><br>[Feb 4](https://discuss.logseq.com/t/how-to-open-any-file-in-the-mobile-app/24864/1)|
|[![](https://discuss.logseq.com/user_avatar/discuss.logseq.com/svartkaffi/144/8001_2.png "svartkaffi")](https://discuss.logseq.com/t/a-hack-for-normalizing-imported-nested-list-of-tabs-from-tree-style-tabs-in-firefox-or-librewolf/20780/1)<br><br>[A hack for normalizing imported nested list of tabs from Tree Style Tabs in Firefox or LibreWolf](https://discuss.logseq.com/t/a-hack-for-normalizing-imported-nested-list-of-tabs-from-tree-style-tabs-in-firefox-or-librewolf/20780)|

|   |
|---|
|[Look what I built](https://discuss.logseq.com/c/customization/look-what-i-built/11)<br><br>[howto](https://discuss.logseq.com/tag/howto)<br><br>[Aug '23](https://discuss.logseq.com/t/a-hack-for-normalizing-imported-nested-list-of-tabs-from-tree-style-tabs-in-firefox-or-librewolf/20780/1)|
|[![](https://discuss.logseq.com/user_avatar/discuss.logseq.com/adxsoft/144/3432_2.png "adxsoft")](https://discuss.logseq.com/t/edit-and-run-python-code-inside-logseq-itself/20829/3)<br><br>[Edit and run python code inside Logseq itself](https://discuss.logseq.com/t/edit-and-run-python-code-inside-logseq-itself/20829)|

|   |
|---|
|[Look what I built](https://discuss.logseq.com/c/customization/look-what-i-built/11)<br><br>[Oct '23](https://discuss.logseq.com/t/edit-and-run-python-code-inside-logseq-itself/20829/3)|
|[![](https://discuss.logseq.com/letter_avatar_proxy/v4/letter/f/cc9497/144.png "fegfeg")](https://discuss.logseq.com/t/apple-shortcuts-logseq-reminders-sync/24055/4)<br><br>[(Apple Shortcuts) Logseq Reminders Sync](https://discuss.logseq.com/t/apple-shortcuts-logseq-reminders-sync/24055)|

|   |
|---|
|[Look what I built](https://discuss.logseq.com/c/customization/look-what-i-built/11)<br><br>[19d](https://discuss.logseq.com/t/apple-shortcuts-logseq-reminders-sync/24055/4)|
|[![](https://discuss.logseq.com/user_avatar/discuss.logseq.com/updog/144/9070_2.png "updog")](https://discuss.logseq.com/t/i-recreated-papaly-the-bookmark-manager-in-logseq-whiteboard-d-heres-how-whiteboards-can-be-improved-to-make-them-10x-as-powerful/26942/1)<br><br>[I recreated Papaly, the bookmark manager in Logseq whiteboard :D Here’s how whiteboards can be improved to make them 10x as powerful](https://discuss.logseq.com/t/i-recreated-papaly-the-bookmark-manager-in-logseq-whiteboard-d-heres-how-whiteboards-can-be-improved-to-make-them-10x-as-powerful/26942)|

|   |
|---|
|[Look what I built](https://discuss.logseq.com/c/customization/look-what-i-built/11)<br><br>[whiteboard](https://discuss.logseq.com/tag/whiteboard)<br><br>[May 7](https://discuss.logseq.com/t/i-recreated-papaly-the-bookmark-manager-in-logseq-whiteboard-d-heres-how-whiteboards-can-be-improved-to-make-them-10x-as-powerful/26942/1)|

### Want to read more? Browse other topics in [Look what I built](https://discuss.logseq.com/c/customization/look-what-i-built/11) or [view latest topics](https://discuss.logseq.com/latest).