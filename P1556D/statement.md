## Description

<div><center> <img class="tex-graphics" height="302px" src="file://yGOZNhkl.png" style="max-width: 100.0%;max-height: 100.0%;" width="454px"> </center><p><span class="tex-font-style-bf">This is an interactive task</span></p><p>William has a certain sequence of integers $a_1, a_2, \dots, a_n$ in his mind, but due to security concerns, he does not want to reveal it to you completely. William is ready to respond to no more than $2 \cdot n$ of the following questions:</p><ul> <li> What is the result of a <a href="https://en.wikipedia.org/wiki/Bitwise_operation#AND">bitwise AND</a> of two items with indices $i$ and $j$ ($i \neq j$) </li><li> What is the result of a <a href="https://en.wikipedia.org/wiki/Bitwise_operation#OR">bitwise OR</a> of two items with indices $i$ and $j$ ($i \neq j$) </li></ul><p>You can ask William these questions and you need to find the $k$-th smallest number of the sequence.</p><p>Formally the $k$-th smallest number is equal to the number at the $k$-th place in a 1-indexed array sorted in non-decreasing order. For example in array $[5, 3, 3, 10, 1]$ $4$th smallest number is equal to $5$, and $2$nd and $3$rd are $3$.</p></div><div class="input-specification"><p>It is guaranteed that for each element in a sequence the condition $0 \le a_i \le 10^9$ is satisfied.</p></div><div><h2>Interaction</h2><p>In the first line you will be given two integers $n$ and $k$ $(3 \le n \le 10^4, 1 \le k \le n)$, which are the number of items in the sequence $a$ and the number $k$.</p><p>After that, you can ask no more than $2 \cdot n$ questions (not including the "<span class="tex-font-style-tt">finish</span>" operation).</p><p>Each line of your output may be of one of the following types: </p><ul> <li> "<span class="tex-font-style-tt">or i j</span>" $(1 \le i, j \le n, i \neq j)$, where $i$ and $j$ are indices of items for which you want to calculate the bitwise <span class="tex-font-style-tt">OR</span>. </li><li> "<span class="tex-font-style-tt">and i j</span>" $(1 \le i, j \le n, i \neq j)$, where $i$ and $j$ are indices of items for which you want to calculate the bitwise <span class="tex-font-style-tt">AND</span>. </li><li> "<span class="tex-font-style-tt">finish res</span>", where $res$ is the $k$th smallest number in the sequence. After outputting this line the program execution must conclude. </li></ul><p>In response to the first two types of queries, you will get an integer $x$, the result of the operation for the numbers you have selected.</p><p>After outputting a line do not forget to output a new line character and flush the output buffer. Otherwise you will get the "<span class="tex-font-style-tt">Idleness limit exceeded</span>". To flush the buffer use:</p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> in C++ </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal </li><li> for other languages refer to documentation </li></ul><p>If you perform an incorrect query the response will be $-1$. After receiving response $-1$ you must immediately halt your program in order to receive an "<span class="tex-font-style-tt">Incorrect answer</span>" verdict.</p><p><span class="tex-font-style-bf">Hacking</span> </p><p>To perform a hack you will need to use the following format:</p><p>The first line must contain two integers $n$ and $k$ $(3 \le n \le 10^4, 1 \le k \le n)$, which are the number of items in the sequence $a$ and the number $k$.</p><p>The second line must contain $n$ integers $a_1, a_2, \dots, a_n$ $(0 \le a_i \le 10^9)$, the sequence $a$.</p></div>

## Input

<p>It is guaranteed that for each element in a sequence the condition $0 \le a_i \le 10^9$ is satisfied.</p>





```input1
7 6

2

7
```




```output1
and 2 5

or 5 6

finish 5
```



## Note

<p>In the example, the hidden sequence is $[1, 6, 4, 2, 3, 5, 4]$.</p><p>Below is the interaction in the example.</p><p></p><table class="tex-tabular"><tbody><tr><td class="tex-tabular-border-left tex-tabular-text-align-left tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><span class="tex-font-style-bf">Query (contestant's program)</span></td><td class="tex-tabular-border-left tex-tabular-text-align-left tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><span class="tex-font-style-bf">Response (interactor)</span></td><td class="tex-tabular-border-left tex-tabular-text-align-left tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><span class="tex-font-style-bf">Notes</span></td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-left tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">and 2 5</td><td class="tex-tabular-border-left tex-tabular-text-align-left tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">2</td><td class="tex-tabular-border-left tex-tabular-text-align-left tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$a_2=6$, $a_5=3$. Interactor returns bitwise AND of the given numbers.</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-left tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">or 5 6</td><td class="tex-tabular-border-left tex-tabular-text-align-left tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">7</td><td class="tex-tabular-border-left tex-tabular-text-align-left tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$a_5=3$, $a_6=5$. Interactor returns bitwise OR of the given numbers.</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-left tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">finish 5</td><td class="tex-tabular-border-left tex-tabular-text-align-left tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"></td><td class="tex-tabular-border-left tex-tabular-text-align-left tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$5$ is the correct answer. Note that you must find the value and not the index of the kth smallest number.</td></tr></tbody></table> <p></p>
