# AS3 Utils

AS3 Utils package for Sublime Text 2 that enhances the default AS3 package. Still in beta, but everything works so far. I use this every day. I'm waiting to add more features before adding it to the package list of Package Control.

## Imports completions for all Adobe's classes
- You can write the name of the class (eg: Sprite) or the name of the folder (eg: display) and you will get a list of possible matches (eg: import flash.display.Sprite). This is scopped so you only get those compltions inside Package but outside Class.

## Methods completions for all Adobe's methods
  - Write any method name and you will get a list of matches. As there are many duplicated results from different classes I've put the name of the class in the autocomplete list. For example "addChild" will throw different results, most likely you will want to use the one from "DisplayObjectContainer".
  - So far only required parameters are included for those methods, optional parameters are ignored.
  - There are still some conflicts with compeltions from the current file... I got around this by installing the (very useful) All Autocomplete package available through Package Control.
  - I've deliberately not included some classes to remove clutter as the auto completion uses a fuzzy search and sometimes there are many unwanted results. The methods for those classes are included in the completions file, but commented out. If you find there is a method of some class you need, it is certainly there, just uncomment it.

## Properties and Constants completions for all Adobe's classes
- Completions for things such as numChildren, length, etc.
- Completions for things such as events, math constants, textfield autosize, stage quality, etc. Eg: MouseEvent.MOUSE_DOWN

## Some useful snippets
  - <b>Class snippet</b> (trigger: class). It will create the default class structure, and use the name of the file for the class name and the constructor. For example MyClass.as will return MyClass. First save your file and then use the snippet.
  - <b>Function snippet</b> (trigger: function). The access control keywords are "dynamic". The whole list will appear (public/private/protected/internal), but if you type "p" then "public" will get written, "pri" will write "private", etc. Then press tab again to go to the next tab cursor in the snippet.
  - <b>Var snippet</b> (trigger: var). The access control keywords are "dynamic", just like the function snippet.
  - <b>Constant snippet</b> (trigger: const). Works exactly as the Var snippet.
  - <b>Comment block snippet</b> (trigger: block). It will create a nice comment block for visually organizing parts of your code.
  - <b>Trace snippet</b> (trigger: trace)
  - <b>setTimeout snippet</b> (trigger: setTimeout)
  - Many other snippets such as <b>for each</b>, <b>if</b>, <b>for in</b>, etc.

## Other great stuff in progress
  - Some completions and snippets for the AS3 Signals framework (https://github.com/robertpenner/as3-signals)
  - Some completions and snippets for the Tweenlite animation framework (https://www.greensock.com/tweenlite/)

# Next features:
  - Documentation search directly from Sublime Text
  - Optional method parameters completions (I really don't know how to include those...)
  - More completions and snippets for Tweenlite and TweenMax
  - Completions and snippets for AS3 Signals