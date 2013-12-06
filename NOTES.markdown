# Autotools

## The structure

                            [Makefile.am]
                                |
    [configure.ac]          (automake)
        |                       |
     (autoconf)             [Makefile.in]
        |                       |
    [(configure)]  <-----------/
        |
    [Makefile]
        |
      (make)
        |
    [my_program]


## The process

    configure.ac
    Makefile.am

aclocal

    aclocal.m4
    autom4te.cache

autoconf

    configure

automake --add-missing

    Makefile.in
    missing         DEMO: ./missing help2man
    install-sh

./configure --prefix `pwd`/prefix

    config.log
    config.status
    Makefile

make

    my_program

make install

    prefix
