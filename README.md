# vim-projectionist-elixir

Vim file navigation for Elixir projects

[online source][l1]

This plugin supplies quick-nav links for Elixir projects.  It
gives commands to jump between an Elixir source file and it's
associated test.

This plugin is going to work with `mix` projects where source
files are stored under the `lib` directory and corresponding test
files are stored under `test`.  

To work with umbrella projects, you'll need to put a custom
`.projections.json` file in the root directory of your umbrella
project.

Install using `Plug` in your `.vimrc`:

    Plug 'tpope/vim-projectionist'
    Plug 'andyl/vim-projectionist-elixir'

Main commands:

`:A` - open the 'alternate' file

`:AS` - open the 'alternate' file in a split window

`:AV` - open the 'alternate' file in a vertical split window

`:AT` - open the 'alternate' file in another tab

This work is based on Tim Pope's [vim-projectionist][l2] plugin.  

[l1]: https://github.com/andyl/vim-projectionist-elixir
[l2]: https://github.com/tpope/vim-projectionist
