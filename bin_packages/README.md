packages created on a raspberry PI with:

```
PKG=<pkg name>; dpkg -L "$PKG" | grep -v '/\.$' | tar -czvf "$PKG".tgz --no-recursion -T -

example:
PKG=libv4lconvert0; dpkg -L "$PKG" | grep -v '/\.$' | tar -czvf "$PKG".tgz --no-recursion -T -
```
