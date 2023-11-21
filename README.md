# CLI-test-texts
Public domain novels for practising the command line.

This repository contains seven George Eliot novels and seven Charles Dickens novels, downloaded from Project Gutenberg: https://www.gutenberg.org. These texts are in the public domain and are in plain text format.

A caveat with these files is that there are multiple line breaks within paragraphs. This makes working with tools like `grep` easier, because the lines returned are short, but means that paragraph-level information has been lost. So, for example, it would not be possible from these files to discover the average paragraph length of the novels (HTML versions of these novels are available from Project Gutenberg, from which paragraph length could be derived using `wc -w` to count the words and `wc -l` to count the lines, although a bit of text manipulation would be needed to remove line breaks within paragraphs).

The Eliot novels are at the top level of the `texts` directory but the Dickens novels are in a subdirectory called `dickens`. This is to allow easy exploration of the Eliot corpus, with the Dickens corpus as a comparator: in both cases a command can be run on `*.txt`, which will work on the Eliot corpus if the working directory is `texts` and on the Dickens corpus if the working directory is `dickens`.
