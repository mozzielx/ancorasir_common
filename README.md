# Git Autocompletion in OS X Terminal

To get autocompletion of Git commands in your OS X Terminal, download [git-completion.bash](https://raw.github.com/git/git/master/contrib/completion/git-completion.bash) to ~ location (e.g. ~/git-completion.bash), you can do the same with [git-prompt.sh](https://raw.github.com/git/git/master/contrib/completion/git-prompt.sh) to show the current Git branch in your prompt.

Rename the file with a "dot" in front to hide the file

```shell
$ mv git-completion.bash .git-completion.bash
$ mv git-prompt.sh .git-prompt.sh
```

List all hiddent files and check the results

```shell
$ ls -a
```

Then update your .bash_profile:

```shell
$ echo 'source ~/.git-completion.bash' >> ~/.bash_profile
$ echo 'source ~/.git-prompt.sh' >> ~/.bash_profile
```

You can check the .bash_profile with the following line

```shell
$ open .bash_profile
```

Now, restart your Terminal and enjoy!
