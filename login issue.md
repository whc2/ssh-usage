## to log in many different services without input passwd every time.
1. generate ssh keys.
2. store keys, such as *id_rsa.pub* to other sevices
3. edit config
```
Host 10.35
    HostName 192.168.10.35
    User yourid
    IdentityFile ~/.ssh/id_rsa
Host 1.23
    HostName 192.168.1.23
    User yourid
    IdentityFile ~/.ssh/id_rsa
```
4. use short name to login
```
ssh 1.23
```
congratulations!
