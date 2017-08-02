LuaSec 0.6
==========
forked from https://github.com/brunoos/luasec

documentation: https://github.com/brunoos/luasec/wiki

to build you need to install gcc 4 or higher

```bash
-bash-3.2$ gmake solaris
---------------------
** Build for Solaris **
---------------------
gmake[1]: Entering directory `/users/nesterov/luasec-luasec-0.6/src'
gmake[2]: Entering directory `/users/nesterov/luasec-luasec-0.6/src'
gmake[3]: Entering directory `/users/nesterov/luasec-luasec-0.6/src/luasocket'
gmake[3]: Nothing to be done for `all'.
gmake[3]: Leaving directory `/users/nesterov/luasec-luasec-0.6/src/luasocket'
cc -O2 -fPIC -Wall -pedantic -I. -I/usr/include -DWITH_LUASOCKET   -c -o ssl.o ssl.c
In file included from ssl.c:22:
/users/nesterov/lua-5.3.4/src/lua.h:93: warning: ISO C90 does not support 'long long'
/users/nesterov/lua-5.3.4/src/lua.h:96: warning: ISO C90 does not support 'long long'
cc -O -fPIC -shared -L./luasocket -L/usr/lib -o ssl.so x509.o context.o ssl.o -lssl -lcrypto -lluasocket
gmake[2]: Leaving directory `/u/nesterov/luasec-luasec-0.6/src'
gmake[1]: Leaving directory `/u/nesterov/luasec-luasec-0.6/src'
```
