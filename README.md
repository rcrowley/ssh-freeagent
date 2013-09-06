`ssh-freeagent`
===============

Don't you hate it when you leave a command running in a screen, close your laptop, and go home only to find the next day that the command needed your SSH agent?  I do.

`ssh-freeagent` creates a new SSH key pair, authorizes the public key to login to one or more hosts, runs a local command that will be able to SSH to those hosts without hassling with SSH agents, and finally unauthorizes the public key and destroys the private key.

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
