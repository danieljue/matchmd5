matchmd5
========

Given a text file with MD5 hashes in it, it will start from the working directory and recursively check files to see if their MD5 hash matches any of the ones in that text file.


Example Usage:

python matchmd5.py testlist.txt

Replace testlist.txt with any kind of text file (csv, xml, free text, etc) that has MD5 hashes anywhere in it.

Note that it starts traversing from your current working directory, so if you wanted to scan your C:\, you would do (with C:\ as your current directory)

c:\python ./path/to/matchmd5.py ./path/to/the/md5list.txt

Optional flags:

-v will turn on verbose printing

-s 1234 will skip files over 1234 bytes. (useful for skipping large files like swap files,  vm images, etc)
