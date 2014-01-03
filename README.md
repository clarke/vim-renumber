# renumber.vim

## Installation

Using [pathogen]( https://github.com/tpope/vim-pathogen ):

```
git clone https://github.com/clarke/vim-renumber.git ~/.vim/bundle/renumber
```

## Summary

The purpose of this vim plugin is to allow easily reordering of numbered lists. This can be very useful when working with things like [Markdown](http://daringfireball.net/projects/markdown/) or other numbered lists. For example, say you have a list such as:

ToDo:

```
1. Take out the trash
2. Put dirty clothes in the wash
3. Go grocery shopping
```

If you typically purchase trash bags and washing machine soap at the grocery store and realize that you are out of these things so you need to move grocery shopping to the top of the list, you would end up with this list:

```
3. Go grocery shopping
1. Take out the trash
2. Put dirty clothes in the wash
```

In the past, I would record a macro using ctrl-a and/or ctrl-x to increment and decrement the numbers, but I found that somewhat tedious. This vim plugin allows you to highlight all rows in a list and run:

```
call Renumber()
```

This will reorder the numbers in the list so that they are sequential starting from 1.


## TODO
- Better handling of sub-items
    - Right now, only unordered sub-items will be ignored, but it should really ignore all sub-items including ordered sub-lists.

## License

Copyright (c) Clarke Retzer. Distributed under the same terms as Vim itself. See :help license.
