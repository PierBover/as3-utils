as3-utils
=========

AS3 Utils package for Sublime Text 2 that enhances the deafult AS3 package.

So far:
  - Imports completions for all classes
    - You can write the name of the class (eg: Sprite) or the name of the folder (eg: events) and you will get a list of possible matches.
  - Methods completions for all methods
    - Write any method name and you will get a list of matches. As there are many duplicated results from different classes I've put the name of the class. For example "addChild" will throw differetn results, most likely you will want to use the one from "DisplayObjectContainer".
    - So far only required parameters are included in the snippets, optional parameters are ignored.
    - There are still some conflicts with compeltions from the current file...
  - Some useful snippets such as:
    - Class snippet (trigger: class). It will create the default class structure, and use the name of the file for the class name and the constructor. For example MyClass.as will return MyClass. First save your file and then use the snippet.
    - TweenLite snippet (trigger: tweenlite)
    - For each snippet (trigger: each)
    - Var snippet (trigger: var)
    - Comment section divider (trigger: section). It will create a nice comment block for visually organizing your methods (inits, event handlers, other, etc).
    - Trace snippet (trigger: trace)



Next features:
  - Documentation search directly from Sublime Text
  - Events completions (eg: MouseEvent.MOUSE_DOWN)