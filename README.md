### Go-Koans support in Emacs

To install Go mode for emacs check this stack response http://stackoverflow.com/questions/1715464/emacs-lisp-mode-for-go

Go-koans have Emacs function to speed up koans resolvig. Simply put `go-koans.el` file somewhere in your `load-path`
and then

    (require 'go-koans)

into your `init.el` file (helper integrates with great Expand region extension from magnars: https://github.com/magnars/expand-region.el)

next `cd` into your koans directory, open some go file and press `C-c C-r` - Emacs will open file and goto line where error occurs

If your code failed you can see at `*go-koans*` buffer there will be shell output from `go test` command


