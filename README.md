# apache-benchmark-microseond-bin

This repo has a rebuilt binary file for apache benchmark tool ("ab" in short).

As the original one does not support microsecond level timing, which is important for the FAST http request test. I change some part of the code in **ab.c** file and rebuild it.

The bin file "ab-percs" can help you to time the http request time in microsecond, and can provide more interesting percentiles.

{1, 5, 10, 15, 20, 25, 30, 35, 40, 45, 50, 55, 60, 66, 75, 80, 90, 95, 98, 99, 100}

The bin file "ab-us-version" now can help you to time the http request time in microsecond :) (I found that I forgot to change the output: "Percentage of the requests served within a certain time (ms)". Actually, the unit should be **microsecond** here, not **ms (milisecond)**)