This is the fifteenth level in the bandit serires.

This on requires us to remember that in a previous level, the passwords for all the bandits were at:
```bash
$ /etc/bandit_pass
```

Once we get the password from there, the next step is to send the information over to a specific port on our
local machine.

This was done by using telnet:
```bash
$ telnet localhost 30000
```
Once a connection is established, simply put the password into the terminal and viola!
The password for the next level is shown.

On to level 15! 
