Sublime Text 3
==============

This is my Sublime resource center. When I need a clean install, this is a 1-page-has-it-all I go to for all the info. Hope you find it useful. Keep scrolling or jump to a particular section.

- [Package Control](#package-control)
- [Packages](#packages)
    - [Sidebar Enhancements](#sidebar-enhancements)
    - [Bracket Highlighter](#bracket-highlighter)
    - [Auto File Name](#auto-file-name)
    - [NodeJS](#nodejs)
    - [Git](#git)
    - [GitGutter](#gitgutter)
    - [Origami](#origami)
    - [Color Picker](#color-picker)
    - [PlainTasks](#plaintasks)
    - [Emmet](#emmet)
    - [Sublime Linter](#sublime-linter)
    - [Tabs Extra](#tabs-extra)
    - [Default File Type](#default-file-type)
    - [Dictionary​Auto​Complete](#dictionaryautocomplete)
    - [jQuery](#jquery)
    - [VAlign](#valign)
    - [Modific](#modific)
    - [Gutter Color](#gutter-color)
    - [Accessibility (aria)](#accessibility-aria)
    - [Data Converter](#data-converter)
    - [Color Highlighter](#color-highlighter)
    - [Packages: Syntax](#packages-syntax)
        - CSS3, CSS Less(ish), Hayaku - tools for writing CSS faster, SCSS, Stylus, Markdown Editing
        - EJS, Java​Script​Next - ES6 Syntax, List LESS variables, List Stylesheet variables
        - Jekyll, Liquid, HAML, PHP Haml, Jade, Jade Snippets
        - Apache Config, .files
    - [Packages: Utility](#packages-utility)
        - TableEditor, Find++, BetteFindBuffer, More Layouts
        - Inline google translate, Terminal, FileDiffs, Minifier, Keymaps
        - Pretty JSON, JSON Reident, JSON Tree
- [Themes](#themes)
    - [Flatland](#flatland)
    - [Spacegray](#spacegray)
    - [Asphalt](#asphalt)
    - [Misc](#misc-themes)
- [Icon](#icon)
- [Fonts](#fonts)
- [Application Default Location](#application-default-location)
- [Keybindings](#keybindings-mac)
- [Preferences](#usersettings-mac)
- [Links](#links)

***

# [Package Control](https://sublime.wbond.net/installation)
Install WBOND's Package Control to be able to extend the Sublime Text functionality with awesome features.
Copy/Paste the following PY code into the Sublime console.
Hit <kbd>CTRL</kbd> + <kbd>`</kbd> to open the console. 

```python
import urllib.request,os,hashlib; h = '7183a2d3e96f11eeadd761d777e62404' + 'e330c659d4bb41d3bdf022e94cab3cd0'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://sublime.wbond.net/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by) 
```

***

<a id="packages">
# Packages

## [Sidebar Enhancements](https://sublime.wbond.net/packages/SideBarEnhancements) ##
![sidebare](images/sidebar.png)

## [Bracket Highlighter](https://sublime.wbond.net/packages/BracketHighlighter)
![br](images/bracketh.png)

## [Auto File Name](https://sublime.wbond.net/packages/AutoFileName)
Add in User.Settings:
```JSON
"auto_complete_triggers":
[
  {
     "characters": "<",
     "selector": "text.html"
  },
  {
     "characters": "/",
     "selector": "string.quoted.double.html,string.quoted.single.html, source.css"
  }
]
```

## [NodeJS](https://sublime.wbond.net/packages/Nodejs)
![nodejsco](images/nodejs.png)

## [Git](https://sublime.wbond.net/packages/Git)
![gitimg](images/git.png)

## [GitGutter](https://sublime.wbond.net/packages/GitGutter)
![gitgutterimg](images/gitgutter.png)

## [Origami](https://sublime.wbond.net/packages/Origami)
![origami](images/origami.png)

## [Color Picker](https://sublime.wbond.net/packages/ColorPicker)
Mac: <kbd>SUPER ⌘</kbd> + <kbd>SHIFT ⇧</kbd> + <kbd>c</kbd><br/>
Win: <kbd>CTRL ⌃</kbd> + <kbd>SHIFT ⇧</kbd> + <kbd>c</kbd>

![color picker](images/colorp.png)

## [PlainTasks](https://sublime.wbond.net/packages/PlainTasks)

User.Preferences:

```json
{
  "open_tasks_bullet": "☐", // options: - | ❍ | ❑ | ■ | □ | ☐ | ▪ | ▫ | – | — ≡ → › | [ ]
  "done_tasks_bullet": "✔", // options: + | ✓ | ✔ | √ | [x]
  "cancelled_tasks_bullet": "✘", // options: x | ✘ | [-]
  "before_tasks_bullet_margin": 1,
  "date_format": "(%y-%m-%d %H:%M)",
  "done_tag": true, // related to @cancelled as well
  "project_tag": true, // if true - postfix archived task with project tag, if false - prefix
  "archive_name": "Archive:", // make sure it is the unique project name within your todo files
  "indent_after_task": true, // indenting the next line after tasks
  "new_on_top": true, // how to sort archived tasks
  "color_scheme": "Packages/PlainTasks/tasks-dark2.hidden-tmTheme",
  "font_size": 16,
  "font_face": "m+ 1m medium",
  "draw_indent_guides": false,
  "line_numbers": false,
  "gutter": true,
  "margin": 2,
  "tab_size": 2,
  "translate_tabs_to_spaces": true,
  "use_tab_stops": false,
  "match_brackets": false,
  "fold_buttons": true,
  "fade_fold_buttons": false,
  "extensions":
  [
    "TODO",
    "todo",
    "todolist",
    "taskpaper",
    "tasks"
  ]
}
```
![plaint](images/plaintasks.png)
 

## [Emmet](https://sublime.wbond.net/packages/Emmet)

![emmet](images/emmet.gif)

### Available actions

* [Expand Abbreviation](http://docs.emmet.io/actions/expand-abbreviation/) – <kbd>Tab</kbd> or <kbd>Ctrl+E</kbd>
* Interactive “Expand Abbreviation” — <kbd>Ctrl+Alt+Enter</kbd>
* [Match Tag Pair Outward](http://docs.emmet.io/actions/match-pair/) – <kbd>⌃D</kbd> (Mac) / <kbd>Ctrl+,</kbd> (PC)
* [Match Tag Pair Inward](http://docs.emmet.io/actions/match-pair/) – <kbd>⌃J</kbd> / <kbd>Shift+Ctrl+0</kbd>
* [Go to Matching Pair](http://docs.emmet.io/actions/go-to-pair/) – <kbd>⇧⌃T</kbd> / <kbd>Ctrl+Alt+J</kbd>
* [Wrap With Abbreviation](http://docs.emmet.io/actions/wrap-with-abbreviation/) — <kbd>⌃W</kbd> / <kbd>Shift+Ctrl+G</kbd>
* [Go to Edit Point](http://docs.emmet.io/actions/go-to-edit-point/) — <kbd>Ctrl+Alt+→</kbd> or <kbd>Ctrl+Alt+←</kbd>
* [Select Item](http://docs.emmet.io/actions/select-item/) – <kbd>⇧⌘.</kbd> or <kbd>⇧⌘,</kbd> / <kbd>Shift+Ctrl+.</kbd> or <kbd>Shift+Ctrl+,</kbd>
* [Toggle Comment](http://docs.emmet.io/actions/toggle-comment/) — <kbd>⇧⌥/</kbd> / <kbd>Shift+Ctrl+/</kbd>
* [Split/Join Tag](http://docs.emmet.io/actions/split-join-tag/) — <kbd>⇧⌘'</kbd> / <kbd>Shift+Ctrl+`</kbd>
* [Remove Tag](http://docs.emmet.io/actions/remove-tag/) – <kbd>⌘'</kbd> / <kbd>Shift+Ctrl+;</kbd>
* [Update Image Size](http://docs.emmet.io/actions/update-image-size/) — <kbd>⇧⌃I</kbd> / <kbd>Ctrl+U</kbd>
* [Evaluate Math Expression](http://docs.emmet.io/actions/evaluate-math/) — <kbd>⇧⌘Y</kbd> / <kbd>Shift+Ctrl+Y</kbd>
* [Reflect CSS Value](http://docs.emmet.io/actions/reflect-css-value/) – <kbd>⇧⌘R</kbd> / <kbd>Shift+Ctrl+R</kbd>
* [Encode/Decode Image to data:URL](http://docs.emmet.io/actions/base64/) – <kbd>⇧⌃D</kbd> / <kbd>Ctrl+'</kbd>
* Rename Tag – <kbd>⇧⌘K</kbd> / <kbd>Shift+Ctrl+'</kbd>

### [Increment/Decrement Number](http://docs.emmet.io/actions/inc-dec-number/)

* Increment by 1: <kbd>Ctrl+↑</kbd>
* Decrement by 1: <kbd>Ctrl+↓</kbd>
* Increment by 0.1: <kbd>Alt+↑</kbd>
* Decrement by 0.1: <kbd>Alt+↓</kbd>
* Increment by 10: <kbd>⌥⌘↑</kbd> / <kbd>Shift+Alt+↑</kbd>
* Decrement by 10: <kbd>⌥⌘↓</kbd> / <kbd>Shift+Alt+↓</kbd>

## [Sublime Linter](https://sublime.wbond.net/packages/SublimeLinter)
- Linters: [PHP](https://sublime.wbond.net/packages/SublimeLinter-php), [JSHint](https://sublime.wbond.net/packages/SublimeLinter-jshint), [JSON](https://sublime.wbond.net/packages/SublimeLinter-json), [HAML](https://sublime.wbond.net/packages/SublimeLinter-haml), [HTML Tidy](https://sublime.wbond.net/packages/SublimeLinter-html-tidy)

## [Tabs Extra](https://sublime.wbond.net/packages/TabsExtra)

![tabse](images/tabsx.png)

## [Default File Type](https://sublime.wbond.net/packages/Default%20File%20Type)

## [Dictionary​Auto​Complete](https://sublime.wbond.net/packages/DictionaryAutoComplete)

![discta](images/dictac.gif)

## [jQuery](https://sublime.wbond.net/packages/jQuery)

![jq](images/jq.png)

## [VAlign](https://sublime.wbond.net/packages/VAlign)
<kbd>Super ⌘</kbd> + <kbd>\\</kbd> 

## [Modific](https://sublime.wbond.net/packages/Modific)
Highlight lines changed since the last commit (supports Git, SVN, Bazaar, Mercurial and TFS).  

![modific](images/modific1.jpg)

## [Gutter Color](https://sublime.wbond.net/packages/Gutter%20Color)
ImageMagic setup:

```bash
    brew uninstall imagemagick
    brew install imagemagick --with-xz --with-font-config --with-little-cms --with-little-cms2
```  

Configuration (User.Settings):

```JSON
    {
        "convert_path" : "convert"  
    }
```

![gutter](images/gutterc.png)

## [Accessibility (aria)](https://sublime.wbond.net/packages/Accessibility)
![aria](images/aria.gif)

## [Data Converter](https://sublime.wbond.net/packages/DataConverter)
A package for Sublime Text 2 for converting CSV data to other formats.  

### Examples

Turn this:

    NAME,VALUE,FRUIT,DATE
    Alice,10,Apple,"Sep. 12, 2012"
    Bob,11,Blueberry,"Sep. 13, 2012"
    Chris,12,Orange,"Sep. 14, 2012"

into this (Ruby):

```ruby
[{"NAME"=>"Alice", "VALUE"=>10, "FRUIT"=>"Apple", "DATE"=>"Sep. 12, 2012"},
{"NAME"=>"Bob", "VALUE"=>11, "FRUIT"=>"Blueberry", "DATE"=>"Sep. 13, 2012"},
{"NAME"=>"Chris", "VALUE"=>12, "FRUIT"=>"Orange", "DATE"=>"Sep. 14, 2012"}];
```

or this (JSON):

```javascript
[
  {"FRUIT": "Apple", "NAME": "Alice", "VALUE": "10", "DATE": "Sep. 12, 2012"},
  {"FRUIT": "Blueberry", "NAME": "Bob", "VALUE": "11", "DATE": "Sep. 13, 2012"},
  {"FRUIT": "Orange", "NAME": "Chris", "VALUE": "12", "DATE": "Sep. 14, 2012"}
]
```

### Formats supported

* ActionScript
* ASP
* HTML tables
* Gherkin
* JIRA (Atlassian Confluence)
* JSON
* JSON (array of columns)
* JSON (array of rows)
* Javascript object
* MySQL
* Perl
* PHP (two formats)
* Python (list of dicts)
* Python (list of lists)
* Ruby
* text table
* Wiki markup
* XML
* XML (property list)
* XML for data-driven Adobe Illustrator
* YAML


## [Color Highlighter](https://sublime.wbond.net/packages/Color%20Highlighter)
![ch1](http://i.imgur.com/UPmEk09.png)
![ch2](http://sametmax.com/wp-content/uploads/2013/04/hilight-color.gif)

***

# Packages: Syntax

- [CSS3](https://sublime.wbond.net/packages/CSS3)
- [CSS Less(ish)](https://sublime.wbond.net/packages/CSS%20Less%28ish%29)
- [Hayaku - tools for writing CSS faster](https://sublime.wbond.net/packages/Hayaku%20-%20tools%20for%20writing%20CSS%20faster)
- [SCSS](https://sublime.wbond.net/packages/SCSS)
- [Stylus](https://sublime.wbond.net/packages/Stylus)
- [Markdown Editing](https://sublime.wbond.net/packages/MarkdownEditing)
- [EJS](https://sublime.wbond.net/packages/EJS)
- [Java​Script​Next - ES6 Syntax](https://sublime.wbond.net/packages/JavaScriptNext%20-%20ES6%20Syntax)
- [List LESS variables](https://sublime.wbond.net/packages/List%20LESS%20Variables)
- [List Stylesheet variables](https://sublime.wbond.net/packages/List%20stylesheet%20variables)
- [Jekyll](https://sublime.wbond.net/packages/Jekyll)
- [Liquid](https://sublime.wbond.net/packages/Liquid)
- [HAML](https://sublime.wbond.net/packages/Haml)
- [PHP Haml](https://sublime.wbond.net/packages/PHP%20Haml)
- [Jade](https://sublime.wbond.net/packages/Jade)
- [Jade Snippets](https://sublime.wbond.net/packages/Jade%20Snippets)
- [Apache Config](https://sublime.wbond.net/packages/ApacheConf.tmLanguage)
- [.files](https://sublime.wbond.net/packages/Dotfiles%20Syntax%20Highlighting)

***

# Packages: Utility
- [TableEditor](https://sublime.wbond.net/packages/Table%20Editor)
- [Find++](https://sublime.wbond.net/packages/Find%2B%2B)
- [BetteFindBuffer](https://sublime.wbond.net/packages/BetterFindBuffer)
- [Inline google translate](https://sublime.wbond.net/packages/Inline%20Google%20Translate)
- [More Layouts](https://sublime.wbond.net/packages/More%20Layouts)
- [Terminal](https://sublime.wbond.net/packages/Terminal)
- [FileDiffs](https://sublime.wbond.net/packages/FileDiffs)
- [Minifier](https://sublime.wbond.net/packages/Minifier)
- [Keymaps](https://sublime.wbond.net/packages/Keymaps)
- [Pretty JSON](https://sublime.wbond.net/packages/Pretty%20JSON)
- [JSON Reident](https://sublime.wbond.net/packages/JSON%20Reindent)
- [JSON Tree](https://sublime.wbond.net/packages/JsonTree)

***

<a id="themes">
# Themes

## [Flatland](https://sublime.wbond.net/packages/Theme%20-%20Flatland)
User.Prefernces:

```JSON
{
  "theme": "Flatland Dark.sublime-theme",
  "color_scheme": "Packages/Theme - Flatland/Flatland Dark.tmTheme"
}
```

Options:

```
{
  // square file tabs instead of rounded corners
  "flatland_square_tabs": true,

  // Monokai color scheme (SublimeText's default) with Flatland background color
  "color_scheme": "Packages/Theme - Flatland/Flatland Monokai.tmTheme",

  // Ability to change row height of sidebar tree
  // Options: xsmall, small, medium, large, xlarge
  "flatland_sidebar_tree_xsmall" : true
}
```

![theme](images/flatland.png)

***

## [Spacegray](https://sublime.wbond.net/packages/Theme%20-%20Spacegray)
User.Preferences:

```json
{
  "theme": "Spacegray.sublime-theme",
  "color_scheme": "Packages/Theme - Spacegray/base16-ocean.dark.tmTheme"

  "theme": "Spacegray Light.sublime-theme",
  "color_scheme": "Packages/Theme - Spacegray/base16-ocean.light.tmTheme"

  "theme": "Spacegray Eighties.sublime-theme",
  "color_scheme": "Packages/Theme - Spacegray/base16-eighties.dark.tmTheme"
}
```

![theme](images/spacegray.png)

***

## [Asphalt](https://sublime.wbond.net/packages/Theme%20-%20Asphalt)
User.Preferences:

```json
{
    "color_scheme": "Packages/Theme - Asphalt/Asphalt.tmTheme",
    "theme": "Asphalt.sublime-theme",
    
    "theme": "Asphalt-monochrome.sublime-theme",
    "theme": "Asphalt-green.sublime-theme",
    "theme": "Asphalt-blue.sublime-theme",
    "theme": "Asphalt-orange.sublime-theme",
}
```

![theme](images/asphalt.png)

## Misc Themes
- [http://sheerun.github.io/sublime-wombat-theme/](http://sheerun.github.io/sublime-wombat-theme/)
- [https://github.com/raik/st2-pseudo-osx-theme](https://github.com/raik/st2-pseudo-osx-theme)
- [https://github.com/thinkpixellab/flatland](https://github.com/thinkpixellab/flatland)
- [http://netatoo.github.io/phoenix-theme/](http://netatoo.github.io/phoenix-theme/)
- [https://github.com/buymeasoda/soda-theme](https://github.com/buymeasoda/soda-theme)
- [https://github.com/daylerees/colour-schemes](https://github.com/daylerees/colour-schemes)

***

<a id="icon">
# Icon
![ico1](images/icon.png)

[http://dribbble.com/shots/382465-Sublime-Text-2-update-Replacement-Icon](http://dribbble.com/shots/382465-Sublime-Text-2-update-Replacement-Icon)

[http://dribbble.com/search?page=2&q=sublime+text](http://dribbble.com/search?page=2&q=sublime+text)

Mac Location:
```bash
        /Contents/Resources/ and replace sublime text.icns with the icons you found
```

***

<a id="fonts">
# Fonts

### [m+ 1m](http://www.fontsquirrel.com/fonts/M-1m)
![m11](images/fontm.png) 

### [Envy Code R](http://damieng.com/blog/2008/05/26/envy-code-r-preview-7-coding-font-released)
![envy1](images/fontenvy1.png)
![envy2](images/fontenvy2.png)

***

## Application Default Location
```
/Users/idj/Library/Application Support/Sublime Text 3
c:\Users\idj\AppData\Roaming\Sublime Text 3\
```


***

## Keybindings (Mac)
If you are primarly working on a Windows machine and are used to using <kbd>CTRL</kbd> + <kbd>PageUP/DN</kbd> to get to top/bottom of the page, you might want check the following bindings:

```JSON
[
    { "keys": ["f1"], "command": "goto_documentation" },
    { "keys": ["ctrl+shift+t"], "command": "delete_trailing_spaces" },
    { "keys": ["f12"], "command": "reindent"},
    { "keys": ["home"], "command": "move_to", "args": {"to": "bol", "extend": false} },
    { "keys": ["end"], "command": "move_to", "args": {"to": "eol", "extend": false} },
    { "keys": ["shift+home"], "command": "move_to", "args": {"to": "bol", "extend": true} },
    { "keys": ["shift+end"], "command": "move_to", "args": {"to": "eol", "extend": true} },
    { "keys": ["ctrl+home"], "command": "move_to", "args": {"to": "bof", "forward": false} },
    { "keys": ["ctrl+end"], "command": "move_to", "args": {"to": "eof", "forward": true} },
    { "keys": ["shift+ctrl+home"], "command": "move_to", "args": {"to": "bof", "forward": false, "extend": true} },
    { "keys": ["shift+ctrl+end"], "command": "move_to", "args": {"to": "eof", "forward": true, "extend": true} },
    { "keys": ["ctrl+shift+d"], "command": "duplicate_line" },
    { "keys": ["super+ctrl+alt+d"], "command": "find_under_expand" },
    { "keys": ["super+ctrl+alt+q"], "command": "change_quotes" },
    { "keys": ["ctrl+shift+alt+m"], "command": "markdown_preview", "args": {"target": "browser"} },
    { "keys": ["ctrl+shift+up"], "command": "swap_line_up" },
    { "keys": ["ctrl+shift+down"], "command": "swap_line_down" },
    { "keys": ["ctrl+shift+alt+up"], "command": "select_lines", "args": {"forward": false} },
    { "keys": ["ctrl+shift+alt+down"], "command": "select_lines", "args": {"forward": true} },
    { "keys": ["ctrl+forward_slash"], "command": "toggle_comment", "args": { "block": false } },
    { "keys": ["ctrl+alt+forward_slash"], "command": "toggle_comment", "args": { "block": true } },
    { "keys": ["ctrl+v"], "command": "paste_and_indent" },
    { "keys": ["ctrl+e"], "command": "goto_recent" }
]
```

## User.Keybindings (Win)
```JSON
[
    { "keys": ["alt+f"], "command": "goto_definition" },
    { "keys": ["ctrl+shift+t"], "command": "delete_trailing_spaces" },
    { "keys": ["ctrl+shift+alt+t"], "command": "reopen_last_file" },
    { "keys": ["ctrl+tab"], "command": "next_view" },
    { "keys": ["ctrl+shift+tab"], "command": "prev_view" },
]
```

## Keyboard Shortcuts

| Keybord ⌘⌃⌥⇧ | Feature |
| ------------- | ------------- |
| <kbd>CTRL ⌃</kbd> + <kbd>M</kbd> | Jump to matching bracket |
| <kbd>CTRL ⌃</kbd> + <kbd>SHIFT ⇧</kbd> + <kbd>M</kbd> | Select everything within the current brackets |
| <kbd>CTRL ⌃</kbd> + <kbd>SHIFT ⇧</kbd> + <kbd>F</kbd> | Find in files |
| <kbd>ALT ⌥</kbd> + <kbd>F3</kbd> | Select all instances of word |
| <kbd>CTRL ⌃</kbd> + <kbd>SHIFT ⇧</kbd> + <kbd>W</kbd>| Wrap Selection in Tag |
| <kbd>SUPERL ⌘</kbd> + <kbd>'</kbd> | Expand to Quotes |

### Links 2
- [https://gist.github.com/lucasfais/1207002](https://gist.github.com/lucasfais/1207002)
- [http://www.cheatography.com/skrobul/cheat-sheets/sublime-text-2-linux/](http://www.cheatography.com/skrobul/cheat-sheets/sublime-text-2-linux/)



***

<a id="pref1s">
## User.Settings (Mac)
```JSON
{
	"auto_complete_commit_on_tab": true,
	"auto_complete_delay": 500,
	"auto_complete_triggers":
	[
		{
			"characters": "<",
			"selector": "text.html"
		},
		{
			"characters": "/",
			"selector": "string.quoted.double.html,string.quoted.single.html, source.css"
		}
	],
	"binary_file_patterns":
	[
		"*.jpg",
		"*.jpeg",
		"*.png",
		"*.gif",
		"*.ttf",
		"*.tga",
		"*.dds",
		"*.ico",
		"*.eot",
		"*.pdf",
		"*.swf",
		"*.jar",
		"*.zip"
	],
	"bold_folder_labels": true,
	"caret_style": "phase",
	"color_scheme": "Packages/User/Sunburst2 (SL).tmTheme",
	"default_encoding": "UTF-8",
	"detect_indentation": true,
	"dictionary": "Packages/Language - English/en_US.dic",
	"caret_extra_bottom": 2,
	"caret_extra_top": 2,
	"caret_extra_width": 3,
	"wide_caret": true,
	"indent_guide_options": ["draw_normal", "draw_active"],
	"draw_centered": false,
	"draw_indent_guides": true,
	"draw_minimap_border": true,
	"enable_hexadecimal_encoding": true,
	"ensure_newline_at_eof_on_save": false,
	"fade_fold_buttons": true,
	"fallback_encoding": "Western (Windows 1252)",
	"file_exclude_patterns":
	[
		"*.pyc",
		"*.pyo",
		"*.exe",
		"*.dll",
		"*.obj",
		"*.o",
		"*.a",
		"*.lib",
		"*.so",
		"*.dylib",
		"*.ncb",
		"*.sdf",
		"*.suo",
		"*.pdb",
		"*.idb",
		".DS_Store",
		"*.class",
		"*.psd",
		"*.db"
	],
	"find_selected_text": true,
	"font_face": "m+ 1m medium",
	"font_size": 16,
	"gutter": true,
	"highlight_line": true,
	"highlight_modified_tabs": true,
	"ignored_packages":
	[
		"Vintage",
		"Markdown"
	],
	"indent_subsequent_lines": true,
	"indent_to_bracket": true,
	"line_padding_bottom": -3,
	"line_padding_top": -3,
	"margin": 4,
	"match_brackets": true,
	"match_brackets_braces": true,
	"match_brackets_content": true,
	"match_brackets_square": true,
	"match_tags": true,
	"open_files_in_new_window": false,
	"remember_open_files": true,
	"remember_open_folders": true,
	"rulers":
	[
		80
	],
	"save_on_focus_lost": true,
	"scroll_past_end": true,
	"scroll_speed": 3,
	"show_full_path": true,
	"smart_indent": true,
	"tab_completion": true,
	"tab_size": 4,
	"theme": "Flatland Dark.sublime-theme",
	"trailing_spaces_highlight_color": "comment",
	"translate_tabs_to_spaces": true,
	"tree_animation_enabled": true,
	"trim_automatic_white_space": true,
	"trim_trailing_white_space_on_save": true,
	"use_newline_glyph": true,
	"use_raw_line_edit_theme": true,
	"use_tab_stops": true,
	"word_separators": "./\\()\"'-:,.;<>~!@#$%^&*|+=[]{}`~?",
	"word_wrap": "auto"
}
```


***
 
<a id="links">
# Links

## Clean Install/Revert
- [http://www.sublimetext.com/docs/2/revert.html](http://www.sublimetext.com/docs/2/revert.html)

## Making Snippets
- [http://stackoverflow.com/questions/7538939/big-comments-with-sublime-text-2/7590725#7590725](http://stackoverflow.com/questions/7538939/big-comments-with-sublime-text-2/7590725#7590725)
- [http://stackoverflow.com/questions/7538939/big-comments-with-sublime-text-2](http://stackoverflow.com/questions/7538939/big-comments-with-sublime-text-2)

## Settings
- [https://gist.github.com/etrepat/1289965](https://gist.github.com/etrepat/1289965)
- [https://github.com/manikrathee/sublime-text/blob/master/Preferences.sublime-settings](https://github.com/manikrathee/sublime-text/blob/master/Preferences.sublime-settings)
- [http://oliverdavies.co.uk/blog/2012/09/my-sublime-text-2-settings](http://oliverdavies.co.uk/blog/2012/09/my-sublime-text-2-settings)
- [http://sokolovstas.github.io/SublimeWebInspector/](http://sokolovstas.github.io/SublimeWebInspector/)
- [http://dnr.azurewebsites.net/2013/04/productivity-sublime-text-2-plugins/](http://dnr.azurewebsites.net/2013/04/productivity-sublime-text-2-plugins/)
- [https://github.com/vitormil/sublime-text-2-preferences](https://github.com/vitormil/sublime-text-2-preferences)
- [https://gist.github.com/alexcican/5248905](https://gist.github.com/alexcican/5248905)

## Tutorials
- [http://docs.sublimetext.info/en/latest/index.html](http://docs.sublimetext.info/en/latest/index.html)
- [http://opensourcehacker.com/2012/05/11/sublime-text-2-tips-for-python-and-web-developers/#Converting_existing_files_to_use_spaces_instead_of_tabs](http://opensourcehacker.com/2012/05/11/sublime-text-2-tips-for-python-and-web-developers/#Converting_existing_files_to_use_spaces_instead_of_tabs)
- [http://blog.stuartherbert.com/php/2012/02/28/setting-up-sublime-text-2-for-php-development/](http://blog.stuartherbert.com/php/2012/02/28/setting-up-sublime-text-2-for-php-development/)
- [http://net.tutsplus.com/articles/news/perfect-workflow-in-sublime-text-free-course/](http://net.tutsplus.com/articles/news/perfect-workflow-in-sublime-text-free-course/)
- [https://tutsplus.com/lesson/http-requests-within-sublime/](https://tutsplus.com/lesson/http-requests-within-sublime/)
- [https://tutsplus.com/lesson/livereload/](https://tutsplus.com/lesson/livereload/)
- [https://tutsplus.com/lesson/vintage-mode/](https://tutsplus.com/lesson/vintage-mode/)
- [https://tutsplus.com/lesson/sublime-and-markdown-with-marked/](https://tutsplus.com/lesson/sublime-and-markdown-with-marked/)
- [http://net.tutsplus.com/articles/news/perfect-workflow-in-sublime-text-free-course/](http://net.tutsplus.com/articles/news/perfect-workflow-in-sublime-text-free-course/)
- [http://blog.alexmaccaw.com/sublime-text](http://blog.alexmaccaw.com/sublime-text)
- [https://www.youtube.com/watch?v=TZ-bgcJ6fQo](https://www.youtube.com/watch?v=TZ-bgcJ6fQo)
- [http://www.cheatography.com/skrobul/cheat-sheets/sublime-text-2-linux/](http://www.cheatography.com/skrobul/cheat-sheets/sublime-text-2-linux/)

## Misc
- [http://blog.stuartherbert.com/php/2012/02/28/setting-up-sublime-text-2-for-php-development/](http://blog.stuartherbert.com/php/2012/02/28/setting-up-sublime-text-2-for-php-development/)
- [https://github.com/mrmartineau/SublimeTextSetup](https://github.com/mrmartineau/SublimeTextSetup)
- [http://net.tutsplus.com/tutorials/tools-and-tips/sublime-text-2-tips-and-tricks/](http://net.tutsplus.com/tutorials/tools-and-tips/sublime-text-2-tips-and-tricks/)
- [http://net.tutsplus.com/tutorials/tools-and-tips/essential-sublime-text-2-plugins-and-extensions/](http://net.tutsplus.com/tutorials/tools-and-tips/essential-sublime-text-2-plugins-and-extensions/)
- [http://opensourcehacker.com/2012/05/11/sublime-text-2-tips-for-python-and-web-developers/](http://opensourcehacker.com/2012/05/11/sublime-text-2-tips-for-python-and-web-developers/)
- [http://stackoverflow.com/questions/7574502/set-default-syntax-to-different-filetype-in-sublime-text-2/8014142#8014142](http://stackoverflow.com/questions/7574502/set-default-syntax-to-different-filetype-in-sublime-text-2/8014142#8014142)
- [http://stackoverflow.com/questions/7666977/syntax-highlighting-for-jade-in-sublime-text-2](http://stackoverflow.com/questions/7666977/syntax-highlighting-for-jade-in-sublime-text-2)
- [http://stackoverflow.com/questions/9495007/indenting-code-in-sublime-text-2](http://stackoverflow.com/questions/9495007/indenting-code-in-sublime-text-2)
- [http://stackoverflow.com/questions/9499848/sublime-text-2-code-snippet](http://stackoverflow.com/questions/9499848/sublime-text-2-code-snippet)
- [http://stackoverflow.com/questions/7476220/image-source-completion-for-sublime-text-2](http://stackoverflow.com/questions/7476220/image-source-completion-for-sublime-text-2)
