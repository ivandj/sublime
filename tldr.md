Sublime Text 3 - TL:DR;
=======================

# Location
```
/Users/idj/Library/Application Support/Sublime Text 3
c:\Users\idj\AppData\Roaming\Sublime Text 3\
```

   
# [Package Control](https://sublime.wbond.net/installation)

```python
import urllib.request,os,hashlib; h = '7183a2d3e96f11eeadd761d777e62404' + 'e330c659d4bb41d3bdf022e94cab3cd0'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://sublime.wbond.net/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by) 
```


# User.Settings (Mac)
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
		"Vintage"
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

# User.Keybindings (Mac)
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

# User.Keybindings (Win)
```JSON
[
    { "keys": ["alt+f"], "command": "goto_definition" },
    { "keys": ["ctrl+shift+t"], "command": "delete_trailing_spaces" },
    { "keys": ["ctrl+shift+alt+t"], "command": "reopen_last_file" },
    { "keys": ["ctrl+tab"], "command": "next_view" },
    { "keys": ["ctrl+shift+tab"], "command": "prev_view" },
]
```

***

# Packages

- [Sidebar Enhancements](https://sublime.wbond.net/packages/SideBarEnhancements)
- [Bracket Highlighter](https://sublime.wbond.net/packages/BracketHighlighter)
- [Auto File Name](https://sublime.wbond.net/packages/AutoFileName)
- [NodeJS](https://sublime.wbond.net/packages/Nodejs)
- [PlainTasks](https://sublime.wbond.net/packages/PlainTasks)
- [Emmet](https://sublime.wbond.net/packages/Emmet)
- [Sublime Linter](https://sublime.wbond.net/packages/SublimeLinter)
    - Linters: [PHP](https://sublime.wbond.net/packages/SublimeLinter-php), [JSHint](https://sublime.wbond.net/packages/SublimeLinter-jshint), [JSON](https://sublime.wbond.net/packages/SublimeLinter-json), [HAML](https://sublime.wbond.net/packages/SublimeLinter-haml), [HTML Tidy](https://sublime.wbond.net/packages/SublimeLinter-html-tidy)
- [Tabs Extra](https://sublime.wbond.net/packages/TabsExtra)
- [Default File Type](https://sublime.wbond.net/packages/Default%20File%20Type)
- [Dictionary​Auto​Complete](https://sublime.wbond.net/packages/DictionaryAutoComplete)
- [jQuery](https://sublime.wbond.net/packages/jQuery)
- [VAlign](https://sublime.wbond.net/packages/VAlign)
- [Modific](https://sublime.wbond.net/packages/Modific)
- [Gutter Color](https://sublime.wbond.net/packages/Gutter%20Color)
- [Accessibility (aria)](https://sublime.wbond.net/packages/Accessibility)
- [Data Converter](https://sublime.wbond.net/packages/DataConverter)

***

# Packages: Syntax

- [CSS3](https://sublime.wbond.net/packages/CSS3)
- [CSS Less(ish)](https://sublime.wbond.net/packages/CSS%20Less%28ish%29)
- [SCSS](https://sublime.wbond.net/packages/SCSS)
- [Stylus](https://sublime.wbond.net/packages/Stylus)
- [EJS](https://sublime.wbond.net/packages/EJS)
- [Java​Script​Next - ES6 Syntax](https://sublime.wbond.net/packages/JavaScriptNext%20-%20ES6%20Syntax)
- [Liquid](https://sublime.wbond.net/packages/Liquid)
- [HAML](https://sublime.wbond.net/packages/Haml)
- [PHP Haml](https://sublime.wbond.net/packages/PHP%20Haml)
- [Jade](https://sublime.wbond.net/packages/Jade)
- [Jade Snippets](https://sublime.wbond.net/packages/Jade%20Snippets)
- [Apache Config](https://sublime.wbond.net/packages/ApacheConf.tmLanguage)
- [.files](https://sublime.wbond.net/packages/Dotfiles%20Syntax%20Highlighting)

***

# Packages: Utility
- [Terminal](https://sublime.wbond.net/packages/Terminal)
- [FileDiffs](https://sublime.wbond.net/packages/FileDiffs)
- [Minifier](https://sublime.wbond.net/packages/Minifier)
- [Keymaps](https://sublime.wbond.net/packages/Keymaps)
- [Pretty JSON](https://sublime.wbond.net/packages/Pretty%20JSON)
- [JSON Reident](https://sublime.wbond.net/packages/JSON%20Reindent)
- [JSON Tree](https://sublime.wbond.net/packages/JsonTree)

***

# Themes

## [Flatland](https://sublime.wbond.net/packages/Theme%20-%20Flatland)

User.Prefernces:

```JSON
{
  "theme": "Flatland Dark.sublime-theme",
  "color_scheme": "Packages/Theme - Flatland/Flatland Dark.tmTheme"
}
```

***

## [Spacegray](https://sublime.wbond.net/packages/Theme%20-%20Spacegray)

User.Prefernces:

```json
{
  "theme": "Spacegray.sublime-theme",
  "color_scheme": "Packages/Theme - Spacegray/base16-ocean.dark.tmTheme"
}
```

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

***

## Misc Themes
- [http://sheerun.github.io/sublime-wombat-theme/](http://sheerun.github.io/sublime-wombat-theme/)
- [https://github.com/raik/st2-pseudo-osx-theme](https://github.com/raik/st2-pseudo-osx-theme)
- [https://github.com/thinkpixellab/flatland](https://github.com/thinkpixellab/flatland)
- [http://netatoo.github.io/phoenix-theme/](http://netatoo.github.io/phoenix-theme/)
- [https://github.com/buymeasoda/soda-theme](https://github.com/buymeasoda/soda-theme)
- [https://github.com/daylerees/colour-schemes](https://github.com/daylerees/colour-schemes)

***

# Icon
![ico1](https://d13yacurqjgara.cloudfront.net/users/2516/screenshots/357612/sublimetext2.jpg)
[http://dribbble.com/shots/382465-Sublime-Text-2-update-Replacement-Icon](http://dribbble.com/shots/382465-Sublime-Text-2-update-Replacement-Icon)
[http://dribbble.com/search?page=2&q=sublime+text](http://dribbble.com/search?page=2&q=sublime+text)

Mac Location:
```bash
        /Contents/Resources/ and replace sublime text.icns with the icons you found
```

***
# Fonts

- [m+ 1m](http://www.fontsquirrel.com/fonts/M-1m)
- [Envy Code R](http://damieng.com/blog/2008/05/26/envy-code-r-preview-7-coding-font-released)



***
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