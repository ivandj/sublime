Sublime Text 3 - Packages
=========================

# [Package Control](https://sublime.wbond.net/installation)

```python
import urllib.request,os,hashlib; h = '7183a2d3e96f11eeadd761d777e62404' + 'e330c659d4bb41d3bdf022e94cab3cd0'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://sublime.wbond.net/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by) 
```

# Packages

## [Sidebar Enhancements](https://sublime.wbond.net/packages/SideBarEnhancements)
![sidebare](http://dl.dropbox.com/u/43596449/tito/sublime/SideBar/screenshot.png)

## [Bracket Highlighter](https://sublime.wbond.net/packages/BracketHighlighter)
![br](http://dl.dropbox.com/u/342698/BracketHighlighter/Example1.png)

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
![nodejsco](http://i.imgur.com/ZCFcC.png)
 
## [PlainTasks](https://sublime.wbond.net/packages/PlainTasks)
![plaint](http://cl.ly/image/1q100Q212o2Q/ss.png)
 
## [Emmet](https://sublime.wbond.net/packages/Emmet)

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
![tabse](https://dl.dropboxusercontent.com/u/342698/TabsExtra/Menu.png)

## [Default File Type](https://sublime.wbond.net/packages/Default%20File%20Type)

## [Dictionary​Auto​Complete](https://sublime.wbond.net/packages/DictionaryAutoComplete)
![discta](https://lh3.googleusercontent.com/-x4YM7vJ1-W4/UXVsHF5l-oI/AAAAAAAAAVk/in3aQcg7jEI/s872/4.gif)

## [jQuery](https://sublime.wbond.net/packages/jQuery)
![jq](http://i.imgur.com/pASjCdM.png)

## [VAlign](https://sublime.wbond.net/packages/VAlign)
<kbd>Super</kbd> + <kbd>\\</kbd> 

## [Modific](https://sublime.wbond.net/packages/Modific)
Highlight lines changed since the last commit (supports Git, SVN, Bazaar, Mercurial and TFS).  

![modific](http://i.imgur.com/DX8TeJT.jpg)
![modific2](http://i.imgur.com/csCw7.jpg)
![modific3](http://i.imgur.com/siVOXl.jpg)
![modigic4](http://i.imgur.com/sldHNl.jpg)

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

![gutter](https://github.com/ivandj/GutterColor/raw/master/screenshot.png)

## [Accessibility (aria)](https://sublime.wbond.net/packages/Accessibility)
![aria](https://raw.githubusercontent.com/Yago/ST3-Accessibility/master/demo.gif)

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

# Pacakages: Syntax

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

# Packages: Utility
- [Terminal](https://sublime.wbond.net/packages/Terminal)
- [FileDiffs](https://sublime.wbond.net/packages/FileDiffs)
- [Minifier](https://sublime.wbond.net/packages/Minifier)
- [Keymaps](https://sublime.wbond.net/packages/Keymaps)
- [Pretty JSON](https://sublime.wbond.net/packages/Pretty%20JSON)
- [JSON Reident](https://sublime.wbond.net/packages/JSON%20Reindent)
- [JSON Tree](https://sublime.wbond.net/packages/JsonTree)

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

<br/><br/><br/><br/>



# Packages To-Check
- [https://sublime.wbond.net/packages/Asterisk%20Config](https://sublime.wbond.net/packages/Asterisk%20Config)
- [https://sublime.wbond.net/packages/Missing%20Palette%20Commands](https://sublime.wbond.net/packages/Missing%20Palette%20Commands)
- [https://sublime.wbond.net/packages/Find%2B%2B](https://sublime.wbond.net/packages/Find%2B%2B)
- [https://sublime.wbond.net/packages/File%20Navigator](https://sublime.wbond.net/packages/File%20Navigator)
- [http://www.brentmountford.com/tutorials/sublime-text-2-sftp-setup-usage/](http://www.brentmountford.com/tutorials/sublime-text-2-sftp-setup-usage/)

