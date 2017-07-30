This is the eleventh level of the bandit series.

The challenge in this one is that all the letters in the file have been rotated by 13 positions.

While at first this might be complicated, there is an easy solution:
```bash
$ cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m' 
```

The cat print all the words in the text file, while the tr command translates the characters.
all the letters from range A-Z get translated to N-Z and A-M whereas all the letters in range
a-z get transltated to their lowercase equivalent.

This will output the password in the nice format.

On to level 12!
