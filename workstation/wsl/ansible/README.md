# Using ansible for openHAB management
## Using SSH-keys for authentication on openHAB server
```
#
# Create keypair
#
$ ssh-keygen -C ralf@node01
#
# List content
#
$ ssh-keygen -l
Enter file in which the key is (/home/ralf/.ssh/id_rsa): 
2048 SHA256:lxru1/f7MnainErK18vneai/9OPHT9TDspQUVz+Wd2E ralf@LAPTOP-WER (RSA)
#
# copy to openhab server
#
$ ssh-copy-id ralf@node01
/usr/bin/ssh-copy-id: INFO: Source of key(s) to be installed: "/home/ralf/.ssh/id_rsa.pub"
/usr/bin/ssh-copy-id: INFO: attempting to log in with the new key(s), to filter out any that are already installed
/usr/bin/ssh-copy-id: INFO: 1 key(s) remain to be installed -- if you are prompted now it is to install the new keys
ralf@node01's password: 

Number of key(s) added: 1

Now try logging into the machine, with:   "ssh 'ralf@node01'"
and check to make sure that only the key(s) you wanted were added.
```

