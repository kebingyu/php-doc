# phpDocumentor for Vim

Version: 1.0.0

This script is based on [php-doc script for Vim by Tobias Schlitt](http://www.vim.org/scripts/script.php?script_id=1355) with the following enhancements:

* Improve and bug fix variable type checking.
* Handle function signature spans multiple lines.
* Print exceptions thrown in function.

The script currently documents:

* Classes
* Methods/Functions
* Attributes

## Installation

Preferred way is to install through a plugin manager, like pathogen or vbundle. For example, to install through pathogen:

    cd ~/.vim/bundle
    git clone https://github.com/kebingyu/php-doc.git

or 

    cd ~/.vim
    git submodule add https://github.com/kebingyu/php-doc.git  bundle/php-doc

Then in vimrc, add the following:

    inoremap <C-P> <ESC>:call PhpDocSingle()<CR>i
    nnoremap <C-P> :call PhpDocSingle()<CR>
    vnoremap <C-P> :call PhpDocRange()<CR>

This maps `<ctrl>+p` to the documentor function. 

## License

Distributed under the same terms as Vim itself.
