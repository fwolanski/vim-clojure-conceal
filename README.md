Vim Clojure Conceal
===================

Unicode lambdas Clojure using Vim's conceal feature. By default, the plugin
conceals all `defn` statements.
For example:

```clojure
(defn square [x]
  (* x x))
```

becomes:

```clojure
(λ square [x]
  (* x x))
```

It requires at least Vim 7.3 and a unicode font.

### `g:clojure_conceal_extras`

Enabling this option changes `fn`, `defn-`, `letfn`, and `#()` to the
Unicode lambda symbol as well.

This option is not set by default. Set it to `1` to enable it.

Installation
============

Drop clojure.vim to `~/.vim/after/syntax` (Linux/Mac OS X/BSD) or
`~/vimfiles/after/syntax` folder (Windows). Or install with pathogen or vundle
in the usual way.

License
=======

Copyright (c) Filip Wolanski. Distributed under the same terms as Vim itself.
See `:help license`.

