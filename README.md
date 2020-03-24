# Installation

Clone the repo and run the install script:

    git clone https://github.com/buildgroundwork/vim-config.git ~/.vim
    cd ~/.vim
    ./install

# Included plugins

## [ALE](https://github.com/dense-analysis/ale)
ALE (Asynchronous Lint Engine) is a plugin providing linting (syntax checking and semantic errors) while you edit your text files, and acts as a Vim [Language Server Protocol](https://langserver.org) client.

#### Mappings:
- <kbd>Ctrl+j</kbd> / <kbd>Ctrl+Shift+j</kbd> Jump to next/previous error

## [fzf](https://github.com/junegunn/fzf)
🌸 A command-line fuzzy finder

**Note**: The default commands for fzf are `:Files`, `:GFiles`, etc.; we have configured the plugin to add the 'Fzf' prefix to commands to disambiguate with other plugins.

#### Mappings:
- <kbd>leader</kbd><kbd>f</kbd> Fuzzy search for files.  This will ignore any files ignored by git if the current directory is a git repository (`:FzfGFiles`) or search all files if not (`:FzfFiles`).
- <kbd>leader</kbd><kbd>r</kbd><kbd>b</kbd> Fuzzy search open buffers.

## [j-split](https://github.com/mgamba/j-split)
Easily split a single line across multiple lines.

#### Mappings:
- <kbd>leader</kbd><kbd>j</kbd> Split the current line.

## [nerdcommenter](https://github.com/preservim/nerdcommenter)
Vim plugin for intensely nerdy commenting powers.

#### Mappings:
- <kbd>leader</kbd><kbd>/</kbd> Comment/uncomment the current line or selection.

## [nerdtree](https://github.com/preservim/nerdtree)
A tree explorer plugin for vim.

#### Mappings:
- <kbd>\\</kbd><kbd>\\</kbd> Open/close the directory tree.
- <kbd>|</kbd> (<kbd>shift+\\</kbd>) Open the directory tree focused on the file in the active buffer.

## [regreplop](https://github.com/vim-scripts/regreplop.vim)
This plugin provides a operator to replace something(motion/visual) with a
specified register.

#### Mappings:
- <kbd>Ctrl+k</kbd> (followed by a motion) Replace with register

## [ultisnips](https://github.com/sirver/UltiSnips)

The ultimate snippet solution for Vim.

Type the snippet followed by <kbd>tab</kbd><kbd>.</kbd>

#### List of custom snippets (incomplete):
- `f` Add a function definition in JavaScript
- `desc` Add a describe block in RSpec or Jasmine
- `cont` Add a context block in RSpec or Jasmine
- `bef` Add a before block in RSpec or Jasmine
- `it` Add an example in Jasmine

## [undotree](https://github.com/mbbill/undotree)
The undo history visualizer for VIM

#### Mappings:
- <kbd>leader</kbd><kbd>u</kbd> Open the undo tree window.

## [vim-abolish](https://github.com/tpope/vim-abolish)
Easily search for, substitute, and abbreviate multiple variants of a word.

Augments the standard search and replace (`:s`) with a smarter search and replace (`:S`).  Read the documentation on the repo; it's worth it.

## [vim-blockle](https://github.com/jgdavey/vim-blockle)
Brace yourself, it's time to toggle your ruby blocks!

#### Mappings:
- <kbd>leader</kbd><kbd>l</kbd> Convert between `do`/`end` and `{}` ruby blocks.

## [vim-bundler](https://github.com/tpope/vim-bundler)
Lightweight support for Ruby's Bundler.

Add syntax highlighting for bundler, as well as `:Bundle` and `:Bopen` commands.

## [vim-dispatch](https://github.com/tpope/vim-dispatch)
Asynchronous build and test dispatcher

## [vim-endwise](https://github.com/tpope/vim-endwise)
Wisely add "end" in ruby, endfunction/endif/more in vim script, etc.

Automatically inserts 'end' for you in ruby blocks.  That's it.

## [vim-fugitive](https://github.com/tpope/vim-fugitive)
A Git wrapper so awesome, it should be illegal.

Many commands for manipulating git inside vim.

## [vim-gitgutter](https://github.com/airblade/vim-gitgutter)
A Vim plugin which shows a git diff in the gutter (sign column) and stages/undoes hunks and partial hunks.

This will automatically update the symbol line (gutter) of the current buffer with git status.

## [vim-haml](https://github.com/tpope/vim-haml)
Vim runtime files for Haml, Sass, and SCSS.

Updated versions of runtime files that ship with vim.

## [vim-javascript](https://github.com/pangloss/vim-javascript)
Vastly improved JavaScript indentation and syntax support in Vim.

## [vim-js-arrow-function](https://github.com/mvolkmann/vim-js-arrow-function)
Ability to toggle JavaScript functions to-and-from arrow functions and toggle their braces.

#### Mappings
- <kbd>leader</kbd><kbd>l</kbd> Toggle braces on an arrow function

## [vim-json](https://github.com/elzr/vim-json)
A better JSON for Vim: distinct highlighting of keywords vs values, JSON-specific (non-JS) warnings, quote concealing.

## [vim-jsx-pretty](https://github.com/MaxMEllon/vim-jsx-pretty)
JSX and TSX syntax pretty highlighting for vim.

## [vim-rails](https://github.com/tpope/vim-rails)
Ruby on Rails power tools

Lots and lots of Rails-specific features.  It's worth reading the documentation for this one.

## [vim-rake](https://github.com/tpope/vim-rake)
It's like rails.vim without the rails.

Useful for non-Rails projects (e.g. gems).

## [vim-repeat](https://github.com/tpope/vim-repeat)
Enable repeating supported plugin maps with ".".

Allow using the <kbd>.</kbd> command to repeat commands from the surround, and unimpaired plugins.

## [vim-ripgrep](https://github.com/jremmen/vim-ripgrep)
Use RipGrep in Vim and display results in a quickfix list.

Use `:Rg` to search for files.  Similar to `:Ack` and `:Ag`.

## [vim-ruby](https://github.com/vim-ruby/vim-ruby)
Vim/Ruby Configuration Files

Syntax highlighting and indentation for ruby.

## [vim-side-search](https://github.com/ddrscott/vim-side-search)
Search context in Vim in a sidebar using `ag` output.

Use `:SideSearch` or `:SS` to search for files.  Customized to work with ripgrep.

## [vim-slim](https://github.com/slim-template/vim-slim)
Syntax highlighting for the [slim templating language](http://slim-lang.com/).

## [vim-surround](https://github.com/tpope/vim-surround)
Quoting/parenthesizing made simple.

Adds a *surround* action for most motions.  Possibly the greatest text-editing plugin of all time.

## [vim-test](https://github.com/janko/vim-test)
A Vim wrapper for running tests on different granularities.

#### Mappings
- <kbd>Ctrl+n</kbd> (`:TestNearest`) Runs the test nearest to the cursor
- <kbd>Ctrl+f</kbd> (`:TestFile`) Runs all tests in the current file
- <kbd>Ctrl+s</kbd> (`:TestSuite`) Runs the whole test suite.
- <kbd>Ctrl+l</kbd> (`:TestLast`) Runs the last test.
- <kbd>Ctrl+g</kbd> (`:TestVisit`) Visits the test file from which you last run your tests

## [vim-textobj-rubyblock](https://github.com/nelstrom/vim-textobj-rubyblock)
A custom text object for selecting ruby blocks.

Allows selecting ruby blocks using `i` and `a` motions.  For example, `vir` will visually select everything inside the ruby block containing the cursor.

## [vim-textobj-user](https://github.com/kana/vim-textobj-user)
Create your own text objects.

Dependency of vim-textobj-rubyblock.

## [vim-toml](https://github.com/cespare/vim-toml)
Vim syntax for [TOML](https://github.com/toml-lang/toml).

## [vim-unimpaired](https://github.com/tpope/vim-unimpaired)
Pairs of handy bracket mappings.

Several convenient key mappings.  For example, <kbd>[</kbd><kbd>space</kbd> and <kbd>]</kbd><kbd>space</kbd> for inserting newlines, and <kbd>[</kbd><kbd>e</kbd> and <kbd>]</kbd><kbd>e</kbd> for swapping lines.

## [vitality.vim](https://github.com/sjl/vitality.vim)
(Vit)ality is a plugin that makes (V)im play nicely with (i)Term 2 and (t)mux.

Now Vim can save when iTerm 2 loses focus, even if it's inside tmux!

It also handles switching the cursor to a bar shaped one when in insert mode, and restoring it when not.

# Color schemes
- molokai
- solarized
- tomorrow
