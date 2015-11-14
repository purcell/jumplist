# jumplist.el

jumplist.el is Emacs port of jumplist(`Ctrl-O`) in vim.

# Requirements

Emacs 24.3 or higher.

# Installation

install directly:

```sh
$ cd load-path-dir
$ wget https://raw.githubusercontent.com/ganmacs/jumplist/master/jumplist.el
```

After Installation add following to your configuration file(~/.emacs.d/init.el, ~/.emacs etc)

```lisp
(require 'jumplist)
```

## Sample Customize

```lisp
(require 'jumplist)
(global-set-key (kbd "C-<") 'jumplist-previous)
(global-set-key (kbd "C->") 'jumplist-next)
(custom-set-variables
 '(jumplist-hook-commands
   '(helm-swoop dired-jump helm-for-files
     isearch-forward end-of-buffer beginning-of-buffer
     find-file)))
```
