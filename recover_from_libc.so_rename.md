![image](https://github.com/user-attachments/assets/e10fac28-23c0-4b23-afe5-0f6cb23a8510)


Renaming libc.so leads to serious result...


But in the end saved by this trick:

```bash
LD_PRELOAD=/lib64/libc.so.6.old mv /lib64/libc.so.6.old /lib64/libc.so.6
```

If the `LD_PRELOAD` trick doesn't work, you can try [this](https://askubuntu.com/questions/1029337/how-can-i-fix-a-missing-renamed-libc-so-6).