vim-weex-snippets
==================

A set of snippets for Vim to work with Alibaba's [Weex](http://github.com/weex/) library.

Requires [vim-snipmate](https://github.com/garbas/vim-snipmate) or [Ultisnips](https://github.com/SirVer/ultisnips).

Installation
============

Use your preferred Vim plugin installation method.
I like [Vundle](http://github.com/gmarik/vundle), but other options like
[pathogen](https://github.com/tpope/vim-pathogen) should work fine as well.

####SnipMate

If you're using Vundle, and you don't currently have SnipMate, you will need to
add the following to your `.vimrc` (taken from the [SnipMate README](https://github.com/garbas/vim-snipmate/blob/master/README.md)):

```
" vim-weex-snippets:
Bundle "vim-weex/vim-weex-snippets"

" SnipMate and its dependencies:
Bundle "MarcWeber/vim-addon-mw-utils"
Bundle "tomtom/tlib_vim"
Bundle "garbas/vim-snipmate"

" Other sets of snippets (optional):
Bundle "honza/vim-snippets"
```
####Ultisnips

If you prefer to use `vim-weex-snippets` with `Ultisnips`, put this in your .vimrc 
to install using Vundle

````
" vim-weex-snippets:
Bundle "vim-weex/vim-weex-snippets"

" Ultisnips
Bundle "SirVer/ultisnips"

" Other sets of snippets (optional):
Bundle "honza/vim-snippets"
````

Usage
=====

Within any Javascript or Weex file, you should be able to do the following:

(in insert mode)
```
weex<Tab>
```

expanding to

```
<template>
  _
</template>

<script>
var modal   = require('@weex-module/modal');
var stream    = require('@weex-module/stream');
var animation = require('@weex-module/animation');
var dom         = require('@weex-module/dom');
module.exports = {
  data: {},
  init: function () {},
  created: function () {},
  ready: function () {},
  methods: function () {}
}
</script>

<style>
/* Add style to here */
</style>
```

And a bunch of others!
Check `snippets/javascript.snippets` to see the full list.
