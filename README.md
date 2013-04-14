# bist

Control gist files to install.

# install

  curl http://mattak.github.io/bist/install.sh | sh

# commands

## list

    bist list
    > 5333258 ljust

    bist list 5333258
    > ljust

## show

display repository content.

    bist show ljust
    bist show 5333258
    > #!/bin/sh ...

## install

install gist content.

    bist install 5333258

## update

update gist contents.

    bist update

## rehash

installed gist to link bin.

    bist rehash

## rm

remove repository.

    bist rm 5333258


# directory

structure of directory.

    $HOME/.bist/
      |
      |- bin/
          |
          |- apkdump
          |- bist
      |
      |- repos/
          |
          |- 5333258/
              |
              |- ljust

# setup dotfile

write your .bistrc .

    $ cat ~/.bistrc

    # ljust
    bist install 5333258

    # ashot
    bist install 5099636

    ...
    
install to execute followings.

    sh ~/.bistrc

