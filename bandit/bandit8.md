This is the ninth level in the bandit series.

The challenge here is finding a line that only appears once.

The best way to do this is with the following command:
```bash
$ sort data.txt | uniq --count | grep "1 "
```

The sort command sorts the data and groups similar lines together, while the uniq command 
finds only the uniq lines, the --count shows the number of times that line appears, and the grep command looks for
"1 " and filters out the other numbers, only revealing the one that is a unique single line

On to levvel 9!
