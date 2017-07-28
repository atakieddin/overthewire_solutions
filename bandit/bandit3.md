This is the fourth level in the bandit series.

The challenge in this level is reading a hidden file (a file with . as the first character) in a directory.
Vim makes this trivial as it automatically shows the hidden file when using the command:
```bash
$ vim inhere
```

However for the sake of the challenge, a better more common tactic is to use the series below:
```bash
$ cd inhere
$ ls -a
```
This will show you all the files including the hidden ones, in the current directory.

Once the file has been located, using either vim or cat will show you the answer

On to level 4!
