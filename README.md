`ssh-freeagent`
===============

Don't you hate it when you leave a command running in a screen and go home only to find the next day that the command needed your SSH agent?  I do.

Installation
------------

Put `ssh-freeagent` on your `PATH`.

Usage
-----

```sh
ssh-freeagent example.com rcrowley.org sh orchestrate.sh
```

where `orchestrate.sh` might contain

```sh
ssh example.com something-slow
ssh rcrowley.org something-slow
```
