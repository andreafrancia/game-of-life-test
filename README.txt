Test di accettazione per il Game of Life
========================================

Per avviare il test::
    
    ./test <nome-del-programma>

Quando passa non dice niente e l'EXIT code é 0, esempio:

    $ ./test ./fake
    $ echo $?
    0

Quando non passa riporta le differenze:

    $ ./test ./fake-bad
    --- -	2012-03-28 01:03:00.000000000 +0200
    +++ /dev/fd/63	2012-03-28 01:03:00.000000000 +0200
    @@ -1,6 +1,6 @@
     Generation 2:
     4 8
     ........
    -...**...
    -...**...
    +........
    +........
     ........
    $ echo $?
    1 

-EOF




