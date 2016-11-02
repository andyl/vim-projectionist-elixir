# vim-projectionist-elixir

Vim file navigation for Elixir projects

[online source](https://github.com/andyl/vim-projectionist-elixir)

This plugin supplies quick-nav links for Elixir projects.  It
gives commands to jump quickly between an Elixir source file
and it's associated test.

This plugin is going to work with `mix` projects where source files are stored
under the `lib` directory and corresponding test files are stored under `test`.
This is not going to work for 1.2.x Phoenix projects with a separate `web`
directory, but will work with 1.3 Phoenix projects where the `web` directory is
moved under `lib`.

Main commands:

`:A` - open the 'alternate' file

`:AS` - open the 'alternate' file in a split window

`:AV` - open the 'alternate' file in a vertical split window

`:AT` - open the 'alternate' file in another tab

This work is based on Tim Pope's
[vim-projectionist](https://github.com/tpope/vim-projectionist)
plugin.  

