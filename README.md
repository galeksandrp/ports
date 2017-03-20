Platform | File Type | Command
--- | --- | ---
Alpine Linux | APKBUILD | `docker run --rm -ti -v $PWD:/home/ng/package -w /home/ng/package galeksandrp/travistest:docker-alpine`
Arch Linux | PKGBUILD | `docker run --rm -ti -v $PWD:/home/ng/package -w /home/ng/package galeksandrp/travistest:docker-arch`
Cygwin | cygport | `cygport *.cygport all`
MSYS2 mingw64 | PKGBUILD | `MINGW_INSTALLS=mingw64 makepkg-mingw -sLf`
MSYS2 mingw32 | PKGBUILD | `MINGW_INSTALLS=mingw32 makepkg-mingw -sLf`
