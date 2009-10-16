These are [YASnippet](http://yasnippet.googlecode.com/svn/trunk/doc/index.html) templates for Emacs that aid in doing tasks with [Shoulda](http://github.com/thoughtbot/shoulda/tree/master). Shoulda consists of test macros, assertions, and helpers, that are added on to the Test::Unit framework for Ruby. Most of the snippets have been ported from the [Shoulda Textmate Bundle](http://svn.textmate.org/trunk/Review/Bundles/Ruby%20Shoulda.tmbundle/).

These snippets assume the use of YASnippet 0.6.1 or later. 

    ;; example setup
    ;; location of yasnippets
    (add-to-list 'load-path "~/.emacs.d/yasnippet")
    (require 'yasnippet)
    (require 'dropdown-list)
    (setq yas/prompt-functions '( yas/ido-prompt
                                  yas/dropdown-prompt
                                  yas/completing-prompt))
    (yas/initialize)
    
    ;; other snippets
    (yas/load-directory "~/.emacs.d/yasnippet/snippets")
    (yas/load-directory "~/.emacs.d/yasnippets-rails/rails-snippets")
    ;; said shoulda snippets
    (yas/load-directory "~/.emacs.d/yasnippets-shoulda")
    
