# apache-benchmark-microseond-bin

This repo has a binary file for apache benchmark tool ("ab" in short)

As the original one does not support microsecond level timing, which is

important for the FAST http request test. I change some part of the code in

ab.c file and rebuild it.

The bin file "ab-us-version" nnow can help you to time the http request time

in microsecond