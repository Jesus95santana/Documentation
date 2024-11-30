Inside the Public folder of the WordPress installation enter this command to fix
any permissions issues (using sudo may help)

```
find . -type d -exec chmod 755 {} \;
find . -type f -exec chmod 644 {} \;
```