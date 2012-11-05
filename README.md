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
mkdir -p ~/.gittemplate/hooks
curl -o ~/.gittemplate/hooks/pre-commit https://raw.github.com/redbet/git-hooks/master/pre-commit;chmod +x ~/.gittemplate/hooks/pre-commit
curl -o ~/.gittemplate/hooks/ruby_syntax_check https://raw.github.com/redbet/git-hooks/master/ruby_syntax_check;chmod +x ~/.gittemplate/hooks/ruby_syntax_check
git config --global init.templatedir "~/.gittemplate"
</pre>

Remember that any project that you have already cloned will not have this,
unless you also symlink the files to *that* project's .git/hooks directory.
