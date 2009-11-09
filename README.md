Execute JavaScript in TextMate
==============================

This is a TextMate bundle for the excellent [Lyndon][].

1. Get [MacRuby][],
2. Get Lyndon. Do so with [rip][]:
    
        rip install git://github.com/defunkt/lyndon.git
    
    Or rubygems:
    
        [sudo] macgem install lyndon

3. Install Lyndon.tmbundle:

        git clone git://github.com/mislav/Lyndon.tmbundle.git \
          "~/Library/Application Support/TextMate/Bundles"

4. Maximum awesome.

Bundle commands
---------------

Shortcuts are the same as equivalents in Ruby documents:

* ⌘R -- run JavaScript document
* ⌃⇧E -- run line / selection as JavaScript

*(Make sure you have your textmate document set to "JavaScript".)*

Try it on
---------

Here's a sample document:

    function camelize(string){
      return string.replace(/-(.)/g, function(_, c){ return c.toUpperCase() })
    }

    camelize('webkit-border-radius')
    
Hitting ⌘R should produce:

    "WebkitBorderRadius"

You're done.
    
[lyndon]: http://github.com/defunkt/lyndon
[macruby]: http://www.macruby.org/downloads.html
[rip]: http://hellorip.com/about.html