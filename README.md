# vim-projectionist-elixir
this is a fork of [vim-projectionist-elixir][l4]

Vim file navigation for Elixir projects 

This plugin supplies quick-nav links for Elixir projects.  **Alternate File
Navigation** gives commands to jump between an Elixir source file and it's
associated test.  **Related File Navigation** gives commands to jump between
Phoenix controllers, views and templates.

Install using `Plug` in your `.vimrc`:

    Plug 'tpope/vim-projectionist'
    Plug 'c-brenn/fuzzy-projectionist.vim'
    Plug 'dkuku/vim-projectionist-elixir'

See also:
- Andyl's [vim-projectionist-elixir][l4] plugin. It was the base for this project.
- Tim Pope's [vim-projectionist][l2] plugin.  
- Conor Brennan's [fuzzy-projectionist.vim][l3] plugin.


## Alternate File Navigation

'Alternates' are the source code and test file - a one-to-one relationship.

`:A` - open the 'alternate' file

`:AS` - open the 'alternate' file in a split window

`:AV` - open the 'alternate' file in a vertical split window

`:AT` - open the 'alternate' file in another tab

## Related File Navigation

In Phoenix projects, you can jump between 'related' files (controllers /
templates / views).

There are two types of relations:
1) one-to-one relationship, eg `controller -> view`
2) one-to-many relationship, eg `controller => template`

For one-to-one relationships, use the Projectionist `E` commands:

- `:Econtroller`
- `:Eview`

For one-to-many relationships, use the Fuzzy-Projectionist `F` commands:

- `:Ftemplate`

## Working with Umbrella Projects

This plugin is going to work with `mix` projects where source
files are stored under the `lib` directory and corresponding test
files are stored under `test`.  

To work with umbrella projects, you'll need to put a custom
`.projections.json` file in the root directory of your umbrella
project.

To quickly generate a `.projections.json` file for an umbrella
project, see the [ex_projections][l1] project.

[l1]: https://github.com/dkuku/ex_projections
[l2]: https://github.com/tpope/vim-projectionist
[l3]: https://github.com/c-brenn/fuzzy-projectionist.vim
[l4]: https://github.com/andyl/vim-projectionist-elixir
