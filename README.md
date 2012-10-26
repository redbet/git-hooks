git-hooks
=========

Remember that time when *you* committed code to master that had syntax errors in it?
Remember how angry the sys admin was at *you*?

Well, now you don't have to look like an ass anymore....

This will syntax check changed rhtml and rb files before letting you make an ass of yourself.

Dependencies
------------

* Ruby
* git

Installation
------------

<pre>
curl -O ~/.gittemplate/hooks/pre-commit https://raw.github.com/redbet/git-hooks/master/pre-commit
curl -O ~/.gittemplate/hooks/ruby_syntax_check https://raw.github.com/redbet/git-hooks/master/ruby_syntax_check
git config --global init.templatedir "~/.gittemplate"
</pre>

Remember that any project that you have already cloned will not have this,
unless you also copy the files to *that* project's .git/hooks directory (and make them executable)
