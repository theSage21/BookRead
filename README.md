# BookRead

Espeak Manager for reading plaintext books

USAGE
-----

bkrd [TextFileName] [start_at_line]

Control
-------

While the book is being read you can use the following keys to
control the reader.

|Key    |Description
--------|-------------
|<space>|to toggle pause and play. Current sentence will be completed before pause or play.
|p      | print the text of the sentence currently being spoken
|s      | sentence number so that you can see how much is done.
|r      | remember this position and start from this the next time this book is read. If a position is specified, that will be used as a start point instead.
|q      | quit

INFO
----

While reading some things are printed on screen. They are in the
following format:

`[LINE_NO] [%DONE] [TRUNCATED_LINE_TEXT]`


Example
-------

`bkrd myfile.txt` reads the text in myfile.txt
`bkrd myfile.txt 10` reads the text in myfile.txt starting at line 10
`bkrd --help` displays this help and exits 

Files Generated
---------------
BKRD generates one file in your home folder called `.bkrd`

This is the file used to keep track of last read positions
in the books you read.

For example in my laptop, it is the file `/home/arjoonn/.bkrd`
