This is the seventh level in the bandit series.

The challenge here is that the file could be anywhere on the server!

The difference with this challenge is that we know some different information.
We still know the size but we also now know the user and the group the file belongs to.

With this information, the following command will work to find the correct file:
```bash
$ find / -group "bandit6" -user "bandit7" -size 33c -type f
```
It will show all the files that are owned by the bandit6 group and the bandit7 user
while also being 33 bytes in size and a file type

However, it will also show a bunch of "Permission denied" things, to avoid that use the command below
```bash
$ find / -group "bandit6" -user "bandit7" -size 33c -type f 2>/dev/null
```
The ```2>/dev/null``` redirects all the errors ```Permission denied``` to /dev/null which just gets rid of them

The file we are looking should show up, and the password is within

On to level 7! 
