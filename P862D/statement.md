## Description

<div><p>Mahmoud and Ehab are in the fourth stage now.</p><p>Dr. Evil has a hidden binary string of length <span class="tex-span"><i>n</i></span>. He guarantees that there is at least one '0' symbol and at least one '1' symbol in it. Now he wants Mahmoud and Ehab to find a position of any '0' symbol and any '1' symbol. In order to do this, Mahmoud and Ehab can ask Dr. Evil up to <span class="tex-span">15</span> questions. They tell Dr. Evil some binary string of length <span class="tex-span"><i>n</i></span>, and Dr. Evil tells the Hamming distance between these two strings. Hamming distance between 2 binary strings of the same length is the number of positions in which they have different symbols. You can find the definition of Hamming distance in the notes section below.</p><p>Help Mahmoud and Ehab find these two positions.</p><p>You will get <span class="tex-font-style-it">Wrong Answer</span> verdict if </p><ul> <li> Your queries doesn't satisfy interaction protocol described below. </li><li> You ask strictly more than <span class="tex-span">15</span> questions and your program terminated after exceeding queries limit. Please note, that you can do up to <span class="tex-span">15</span> ask queries and one answer query. </li><li> Your final answer is not correct. </li></ul> You will get <span class="tex-font-style-it">Idleness Limit Exceeded</span> if you don't print anything or if you forget to flush the output, including for the final answer (more info about flushing output below).<p>If you exceed the maximum number of queries, You should terminate with 0, In this case you'll get Wrong Answer, If you don't terminate you may receive any verdict because you'll be reading from a closed stream .</p></div><div class="input-specification"><p>The first line of input will contain a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1000</span>)&nbsp;— the length of the hidden binary string.</p></div><div class="output-specification"><p>To print the final answer, print "! pos0 pos1" (without quotes), where <span class="tex-span"><i>pos</i>0</span> and <span class="tex-span"><i>pos</i>1</span> are positions of some '0' and some '1' in the string (the string is 1-indexed). <span class="tex-font-style-bf">Don't forget to flush the output after printing the answer!</span></p></div><div><h2>Interaction</h2><p>To ask a question use the format "? s" (without quotes), where <span class="tex-span"><i>s</i></span> is a query string. <span class="tex-font-style-bf">Don't forget to flush the output after printing a query!</span></p><p>After each query you can read a single integer from standard input&nbsp;— the Hamming distance between the hidden string and the query string.</p><p>To flush the output you can use:- </p><ul> <li> fflush(stdout) in C++; </li><li> System.out.flush() in Java; </li><li> stdout.flush() in Python; </li><li> flush(output) in Pascal; </li><li> See the documentation for other languages . </li></ul><p><span class="tex-font-style-bf">Hacking.</span> </p><p>To hack someone just print one binary string with length up to <span class="tex-span">1000</span>, containing at least one '0' and at least one '1'.</p></div>

## Input

<p>The first line of input will contain a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1000</span>)&nbsp;— the length of the hidden binary string.</p>

## Output

<p>To print the final answer, print "! pos0 pos1" (without quotes), where <span class="tex-span"><i>pos</i>0</span> and <span class="tex-span"><i>pos</i>1</span> are positions of some '0' and some '1' in the string (the string is 1-indexed). <span class="tex-font-style-bf">Don't forget to flush the output after printing the answer!</span></p>





```input1
3
2
1
3
2
1
0
```




```output1
? 000
? 001
? 010
? 011
? 100
? 101
! 2 1
```



## Note

<p>Hamming distance definition: <a href="https://en.wikipedia.org/wiki/Hamming_distance">https://en.wikipedia.org/wiki/Hamming_distance</a></p><p>In the first test case the hidden binary string is 1<span class="tex-font-style-bf">0</span>1, The first query is 0<span class="tex-font-style-bf">0</span>0, so the Hamming distance is <span class="tex-span">2</span>. In the second query the hidden string is still 1<span class="tex-font-style-bf">01</span> and query is 0<span class="tex-font-style-bf">01</span>, so the Hamming distance is <span class="tex-span">1</span>.</p><p>After some queries you find that symbol at position <span class="tex-span">2</span> is '0' and symbol at position <span class="tex-span">1</span> is '1', so you print "! 2 1".</p>
