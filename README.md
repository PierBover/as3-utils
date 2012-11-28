# AS3 Utils

AS3 Utils package for Sublime Text 2 that enhances the default AS3 package. Still in beta, but everything works so far. I use this every day. I'm waiting to add more features before adding it to the package list of Package Control.

## Imports completions for all Adobe classes
- You can write the name of the class (eg: Sprite) or the name of the folder (eg: events) and you will get a list of possible matches. Obviously this only works in the imports section inside package but outside class.

## Methods completions for all Adobe methods
  - Write any method name and you will get a list of matches. As there are many duplicated results from different classes I've put the name of the class in the autocomplete list. For example "addChild" will throw differetn results, most likely you will want to use the one from "DisplayObjectContainer".
  - So far only required parameters are included in the snippets, optional parameters are ignored.
  - There are still some conflicts with compeltions from the current file... I got around this by installing the (very useful) All Autocomplete package available through Package Control.

## Some useful snippets
  - <b>Class snippet</b> (trigger: class). It will create the default class structure, and use the name of the file for the class name and the constructor. For example MyClass.as will return MyClass. First save your file and then use the snippet.
  - Function snippet (trigger: function). The access control keywords are "dynamic". The whole list will appear (public/private/protected/internal), but if you type "pub" "public" will get written, "pri" will write "private", etc. Then press tab again to go to the next tab cursor in the snippet.
  - For each snippet (trigger: for each)
  - Var snippet (trigger: var)
  - Comment section divider (trigger: section). It will create a nice comment block for visually organizing your methods (inits, event handlers, other, etc).
  - Trace snippet (trigger: trace)
  - setTimeout snippet (trigger: setTimeout)

## Other great stuff
  - Some completions and snippets for the AS3 Signals framework (https://github.com/robertpenner/as3-signals)
  - Some completions and snippets for the Tweenlite animation framework (https://www.greensock.com/tweenlite/)

# Next features:
  - Documentation search directly from Sublime Text
  - Events completions (eg: MouseEvent.MOUSE_DOWN)
  - Properties completions
  - Optional method parameters completions
  - Completions for Tweenlite easings
  - Completions and snippets for AS3 Signals