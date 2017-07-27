This is the second challenge in the bandit series.

The challenge of this one is how to read a file called -

- is a special character because it represent the stdin. So doing:

```bash
$ cat -
``` 
or 
```bash
$ vim -
```

Won't prove to be helpful. Instead, we have to use the old school way of specifying file locations
and outline the exact path as below:

```bash
$ vim "./-"
```

or with cat.

Doing this will show us the next password.

On to level 2!
