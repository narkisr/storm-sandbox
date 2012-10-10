# About
This is a vagrant sanbox for [storm](https://github.com/nathanmarz/storm), it includes the puppet module and the fpm-recipe in order to package and install storm.

# Usage

First build zeromq jzmq and storm packages (follow exact order):

```bash 
# install required gems
$ bundle install
# now build packages
$ cd fpm-recipes/zeromq/
$ fpm-cook
$ cd fpm-recipe/jzqm/
$ fpm-cook
$ cd fpm-recipe/storm/
$ fpm-cook
```

Now lets start a nimbus and 2 distributed workers:

```bash 
$ vagrant up
```


