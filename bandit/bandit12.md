This is the thirteenth level in the bandit serires.

The challenge in this one is that we have a hex dump of a file that was repeatedly compressed.

This one is actually quite challenging in that there are a lot of steps.
Below is the complete way I solved this one:
```bash
$ xxd -r data.txt > text
$ file text
$ mv text text.gz
$ gzip -d text.gz
$ file text
$ bzip2 -d text
$ file text.out
$ mv text.out text.gz
$ gzip -d text.gz
$ file text
$ tar -xf text
$ file data5.bin
$ tar -xf data5.bin
$ file data6.bin
$ bzip2 -d data6.bin
$ file data6.bin.out
$ file data8.bin
$ mv data8.bin data8.bin.gz
$ gzip -d data8.bin.gz
$ file data8
$ cat data8
```
And the password should be shown.

On to level 13!
