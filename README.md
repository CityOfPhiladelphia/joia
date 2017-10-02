# joia

Deploy an app to an instance on AWS

```
usage: joia <command>

commands:
  deploy    deploy app on instance
  down      destroy instance
  env       set environment on instance
  host      set up ssh host config for an instance
  install   install app stack on instance
  push      push files to instance
  pull      pull files from instance
  ssh       ssh into instance
  sync      sync files with instance
  up        spin instance up
  watch     sync and deploy on file changes
```


## Install

Dependencies: 
* [aws cli](http://docs.aws.amazon.com/cli/latest/userguide/installing.html)
* cat
* ed
* rsync
* ssh
* unison (on both local and instance if you want to use sync)

Place executable "joia" file in a directory in your $PATH, or symlink the directory. 


## Configuration

Global variables are set in `~/.joiarc`. Good candidates for this file include KEYPAIR and SUBNET.

App-specific variables can be set in `.env` at the root of an app.

## Addtional notes

Create an AWS Access ID with permissions to create and modify ec2 instances. 
