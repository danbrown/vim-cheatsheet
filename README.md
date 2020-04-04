# Vim Commands Cheat Sheet

> This article is under building process, if you want to help, contact me! me@danielbrown.com.br

###

Everyone of us have troubles when editing a file via command line. thats why is so important to learn [Vim Editor](https://www.vim.org/), and thats why I created this repository. Based on [Daniel Gryniewicz]() cheat sheet, inspired by [Ben Awad](https://www.youtube.com/watch?v=4WTV6ZCY4qo) video and [Lucas Montano](https://www.youtube.com/channel/UCyHOBY6IDZF9zOKJPou2Rgg) "Good Programmers have to Type Fast" [ironic quote](https://www.youtube.com/watch?v=ZUWO7x9_8jE) 😜.

## Copying and Moving Text

| Command                   | Result                                                                                                                                            |
| :------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------- |
| "{a-zA-Z0-9.%#:-"}        | Use register {a-zA-Z0-9.%#:-"} for next delete, yank or put (use uppercase character to append with delete and yank) ({.%#:} only work with put). |
| :reg[isters]              | Display the contents of all numbered and named registers.                                                                                         |
| :reg[isters] {arg}        | Display the contents of the numbered and named registers that are mentioned in {arg}.                                                             |
| :di[splay][arg]           | Same as :registers.                                                                                                                               |
| ["x]y{motion}             | Yank {motion} text [into register x].                                                                                                             |
| ["x]yy                    | Yank [count] lines [into register x]                                                                                                              |
| ["x]Y                     | yank [count] lines [into register x] (synonym for yy).                                                                                            |
| {Visual}["x]y             | Yank the highlighted text [into register x] (for {Visual}).                                                                                       |
| {Visual}["x]Y             | Yank the highlighted lines [into register x]                                                                                                      |
| :[range]y[ank][x]         | Yank [range] lines [into register x].                                                                                                             |
| :[range]y[ank][x] {count} | Yank {count} lines, starting with last line number in [range] (default: current line), [into register x].                                         |
| ["x]p                     | Put the text [from register x] after the cursor [count] times.                                                                                    |
| ["x]P                     | Put the text [from register x] before the cursor [count] times.                                                                                   |
| ["x]gp                    | Just like "p", but leave the cursor just after the new text.                                                                                      |
| ["x]gP                    | Just like "P", but leave the cursor just after the new text.                                                                                      |
| :[line]pu[t][x]           | Put the text [from register x] after [line] (default current line).                                                                               |
| :[line]pu[t]! [x]         | Put the text [from register x] before [line] (default current line).                                                                              |

## Writed by

Daniel Brown – [@odanielbrown](https://twitter.com/odanielbrown) – me@danielbrown.com.br
Based on [Daniel Gryniewicz](https://www.fprintf.net/vimCheatSheet.html) cheat sheet

[https://github.com/odanielbrown](https://github.com/odanielbrown/)

## Contributing

1. Fork it (<https://github.com/odanielbrown/vim-cheatsheet/fork>)
2. Create your feature branch (`git checkout -b feature/fooBar`)
3. Commit your changes (`git commit -am 'Add some fooBar'`)
4. Push to the branch (`git push origin feature/fooBar`)
5. Create a new Pull Request
