freq
====

Simple command that takes lines as input and output the number of lines
received during one second. Example:

    $ yes | freq
    1031638 lines/sec
    1031801 lines/sec
    1031613 lines/sec

What is it useful for?
----------------------

The main problem I was trying to solve, and I wanted the information fast, was
to determine how many requests per second my webserver was handling. It was
something like this:

    $ tail -f /var/log/foo.log | freq
    945 lines/sec
    862 lines/sec
    902 lines/sec

If you happen to find another cool use for this, just let me know :)
