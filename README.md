# integration/php-coveralls.git

This repository holds php-coveralls and its dependencies.
See https://github.com/satooshi/php-coveralls
It is meant to safely deploy php-coveralls on the Wikimedia cluster since:

1) we can NOT download from third parties
2) there is no Debian package for php-coveralls

## How to update

Use http://getcomposer.org/ a package management system for PHP.

Review composer.json, update the version and update:

    $ composer update

REVIEW THE DIFF!

    $ git diff

If it looks sane, add and commit for review:

    $ git add -A
    $ git commit -m 'Updating php-coveralls to vX.X.X'
    $ git push refs/for/master
    ..
    $

Then ask for review.
