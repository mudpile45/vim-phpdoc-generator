vim-phpdoc-generator
====================

Update and generate phpdoc vim help files for vim-phpdoc

Idea, code and directions taken from [Fumbling In The
Dark](http://www.fumbling-in-the-dark.com/2011/03/viewing-php-manual-in-vim.html).

To regenerate the phpdocs use the following commands:
``svn co http://svn.php.net/repository/phpdoc/modules/doc-en phpdoc
find . -name "reference" -print > references.txt
find . -name "*.ent" -print > ent.txt
mkdir out 
php parser.php``

and put the results in your vim plugin folder. 

See [vim-phpdoc](https://github.com/mudpile45/vim-phpdoc) for more info on how
to use the plugin
