# Configure your ssh client
In your home directory you can find a directory called `.ssh`, in this directory you can find all the needed config for your commandline client.
If you have ever made a connection to an ssh server, you will find a file `known_hosts`. This file keeps record of all the servers to which you have connected in the past, if something changes on the server e.g. the ip-address the ssh client will warn you about this change. 

If the directory `.ssh` doesn't exist, it can be created by:
```shell
mkdir ~/.ssh
chmod 700 ~/.ssh
```

## Create config file
The config file of your ssh client enables you to configure your preferences on the client side.

```shell
cd ~/.ssh
touch config
```

Change the defaults of the following snippet and insert it in the previously created config file.
```shell
Host gitserver
        User git
        Hostname yourserver.com
        Port 2222
        IdentityFile ~/.ssh/id_rsa.gitserver.pub
```

## Create key
You can increase the security of your key by entering a passphrase. It is considered less secure not providing a passphrase.
```shell
ssh-keygen -t rsa -b 4096 -C "your name and/or id and/or some comment" -f ~/.ssh/id_rsa.gitserver
```

## SSH client is ready
The ssh client is now ready, you can now continue with the gitserver manual.
