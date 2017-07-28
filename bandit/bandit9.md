This is the tenth level in the bandit series.

The challenge here is that we must find the only human readable string and there is a series of '=' near it.
Looking at data.txt however we can see that it is a data file with the following command:
```bash
$ file data.txt
```
We can use the strings command to filter through all the data in the data file and find the string values
Since we have a lot of strings we need to filter it to look for the something that starts with a series of '='
Using the following command we find the correct password.
```bash
$ strings data.txt | grep "="
```
The password would then be returned

On to level 10!
