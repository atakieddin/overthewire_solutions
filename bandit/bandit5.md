This is the sixth level in the bandit series.

This one is similar to the last one, except this time the file could be in any number of directories.

Luckily we have some hints to help guide us.

The only hint we really need to solve this challenge however is the size 1033.
Using the below command we can find the file we are looking for, based on sized
```bash
$ du -ab ./maybehere**/* | grep "1033"
```

The part before the pipe will show all the files and their sizes in bytes, where using the grep after the pipe will filter
the results to only files with size 1033. Luckily for us there is only one.

Viewing this file will show us the password.

On to level 6!
