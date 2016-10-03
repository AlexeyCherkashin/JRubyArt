---
layout: post
title:  "Editors and Other Resources"
date:   2015-10-24 08:07:00
categories: jruby_art update
permalink: /editors/
keywords: editor, ide, ruby, jruby_art, vim, emacs, jedit
---
### Atom ###

If you are a millenial (never used emacs, vim or jedit), then atom will blow your mind, install atom-k9 for JRubyArt but you can run sketches in either `k9 --run` or `k9 --watch` mode see [JRubyArt with atom][atom]. Edit the file in atom and save and the sketch will reload to reflect your changes...

![atom-watch]({{ site.github.url }}/assets/jwishy.png)

### Textmate / Sublime Text
A very simple [Textmate Bundle][textmate] was created to run ruby-processing projects in textmate, which could be adapted for JRubyArt (please share your experience)

### JEdit
Alternatively install my jEdit [k9.xml][commando] commando file. Full [instructions here][jedit] to `run`/`watch` JRubyArt sketches all from the jEdit ide/editor (Windows users should be most interested in this). Can be used as `pry` editor

![jEdit]({{ site.github.url }}/assets/jedit.png)

### Vim
Is an excellent choice for linux and mac users, commands available from vim:-
{% highlight bash %}
:!k9 --run %   # will run the sketch
k9 --live %  # to create a pry repl do not do this from vim
:!k9 --watch % # reloads and run sketch on save
{% endhighlight %}
see [live editing with pry][pry]. Sketches created with `template: class` work best for live editing.

### Emacs
Similar to vim (also works well with pry see [detailed instructions][pry]). Emacs can also be heavily [customised][emacs] use the `template: emacs` setting to create sketches for the customised emacs.

### Netbeans
There is even a [plugin for NetBeans][plugin] (by the jruby guys, well probably just Tom Enebo) for the really serious. You can load the `jruby_art` gem from netbeans, but currently you may need a manual install of JRuby-9.1.5.0. Sketches created with the `template: emacs` setting can be run from the ide.

[atom]:{{site.github.url}}/atom
[plugin]:https://plugins.netbeans.org/plugin/38549
[textmate]:https://github.com/tibastral/ruby-processing-tmbundle
[jedit]:https://monkstone.github.io/jedit4processing/jekyll/update/2015/12/11/welcome.html
[emacs]:https://github.com/ruby-processing/JRubyArt/wiki/Using-emacs-as-your-JRubyArt-Ide
[commando]:https://github.com/monkstone/jedit4processing/blob/master/.jedit/console/commando/k9.xml
[pry]:https://github.com/ruby-processing/JRubyArt/wiki/Live-Coding