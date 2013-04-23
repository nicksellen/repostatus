repostatus
==========

command line tool for checking the status of git/svn repositories

Shows you:

type of repository [whether you have a remote] | number of changes not committed | path to repo

Ordered by number of uncommited changes ascending and runs from the current directory (it descends into all the child directories). It can be a bit slow with lots of repos.

Example usage and output
---------

# repostatus 
git !remote      0 example/project/without/a/remote
git !remote      1 another/but/with/one/uncommited/change
svn             15 a/nice/svn/project/too
git             87 this/really/needs/some/committing
