# mu4e contribution layer for Spacemacs

mu4e is an Emacs frontend for the [mu](http://www.djcbsoftware.nl/code/mu/) mail
indexer.

## Getting Started

Follow
[mu4e's](http://www.djcbsoftware.nl/code/mu/mu4e/Getting-started.html#Getting-started)
directions to get started. Take heart, once setup it's clear sailing.

### Personal Config

The mu4e layer calls `dotmu4e/init` on initial configuration, and
`dotmu4e/config` at the end of configuration.

Here is a basic example of `dotmu4e/init`:

```elisp
(defun dotmu4e/init ()
  (setq-default
    mu4e-maildir     "/home/user/Maildir"
    mu4e-sent-folder "/path/to/sent/folder"
))
```

mu4e has sensible variable defaults. See `mu4e-vars.el` for all mu4e variables
with descriptions.

## Key bindings

Most existing bindings remain the same, with the exception of those traded for
`hjkl` compatibility. `C-{j,k}` will take you to the next/prev message in
headers and view mode.

and `mu4e-view-mode`

`mu4e-main-mode`

Key Binding          |                 Description
---------------------|------------------------------------------------------
<kbd>J</kbd>         | `mu4e~headers-jump-to-maildir`

`mu4e-headers-mode`

Key Binding          |                 Description
---------------------|------------------------------------------------------
<kbd>J</kbd>         | `mu4e~headers-jump-to-maildir`
<kbd>C-j</kbd>       | `mu4e-headers-next`
<kbd>C-k</kdb>       | `mu4e-headers-prev`

`mu4e-view-mode`

Key Binding          |                 Description
---------------------|------------------------------------------------------
<kbd>J</kbd>         | `mu4e~headers-jump-to-maildir`
<kbd>C-j</kbd>       | `mu4e-view-headers-next`
<kbd>C-k</kdb>       | `mu4e-view-headers-prev`
