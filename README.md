# print-on-nums11
How to move files to nums11 server and print them.

1. Copy file from local directory to the numerik server:
``` bash
scp 'path-to-your-local-file/your-file' 'your-user'@nums11.zib.de:'path-to-your-remote-directory'
```

2. Log into numerik server via ssh:
``` bash
ssh 'your-user'@nums11.zib.de
```

3. Print the file (e.g. on panda (color) or bee (b/w))
``` bash
cd 'path-to-your-remote-directory'
lpr -P panda 'your-file'
```

3.a If you like, check the print status:
``` bash
lpq -P panda
```
