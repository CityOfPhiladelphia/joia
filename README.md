# joia

Deploy an app to an instance on AWS

```
usage: joia <command>

commands:
  deploy    deploy app on instance
  down      destroy instance
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

Dependencies: aws, cat, ed, rsync, ssh (and unison on both local and instance if you want to use sync)

Place executable "joia" file in a directory in your $PATH.
