Sublime Text 3 - Settings
=========================

# Location
```
/Users/idj/Library/Application Support/Sublime Text 3
c:\Users\idj\AppData\Roaming\Sublime Text 3\
```

# Keyboard Shortcuts

| Keybord ⌘⌃⌥⇧ | Feature |
| ------------- | ------------- |
| <kbd>CTRL ⌃</kbd> + <kbd>M</kbd> | Jump to matching bracket |
| <kbd>CTRL ⌃</kbd> + <kbd>SHIFT ⇧</kbd> + <kbd>M</kbd> | Select everything within the current brackets |
| <kbd>CTRL ⌃</kbd> + <kbd>SHIFT ⇧</kbd> + <kbd>F</kbd> | Find in files |
| <kbd>ALT ⌥</kbd> + <kbd>F3</kbd> | Select all instances of word |
| <kbd>CTRL ⌃</kbd> + <kbd>SHIFT ⇧</kbd> + <kbd>W</kbd>| Wrap Selection in Tag |
| <kbd>SUPERL ⌘</kbd> + <kbd>'</kbd> | Expand to Quotes |
    
### Links
- [https://gist.github.com/lucasfais/1207002](https://gist.github.com/lucasfais/1207002)
- [http://www.cheatography.com/skrobul/cheat-sheets/sublime-text-2-linux/](http://www.cheatography.com/skrobul/cheat-sheets/sublime-text-2-linux/)


# [Package Control](https://sublime.wbond.net/installation)

```python
import urllib.request,os,hashlib; h = '7183a2d3e96f11eeadd761d777e62404' + 'e330c659d4bb41d3bdf022e94cab3cd0'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://sublime.wbond.net/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by) 
```

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

## User.Keybindings (Mac)
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
