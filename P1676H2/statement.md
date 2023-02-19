## Description

<div><p><span class="tex-font-style-it">The only difference between the two versions is that in this version</span> $n \leq 2 \cdot 10^5$ and the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$<span class="tex-font-style-it">.</span></p><p>A <span class="tex-font-style-it">terminal</span> is a row of $n$ equal segments numbered $1$ to $n$ in order. There are two terminals, one above the other. </p><p>You are given an array $a$ of length $n$. For all $i = 1, 2, \dots, n$, there should be a straight wire from some point on segment $i$ of the top terminal to some point on segment $a_i$ of the bottom terminal. You can't select the endpoints of a segment. For example, the following pictures show two possible wirings if $n=7$ and $a=[4,1,4,6,7,7,5]$.</p><center> <img class="tex-graphics" src="file://eN7upnJJ.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>A <span class="tex-font-style-it">crossing</span> occurs when two wires share a point in common. In the picture above, crossings are circled in red.</p><p>What is the <span class="tex-font-style-bf">maximum</span> number of crossings there can be if you place the wires optimally?</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 2 \cdot 10^5$)&nbsp;— the length of the array.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \leq a_i \leq n$)&nbsp;— the elements of the array.</p><p>The sum of $n$ across all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;— the <span class="tex-font-style-bf">maximum</span> number of crossings there can be if you place the wires optimally.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 2 \cdot 10^5$)&nbsp;— the length of the array.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \leq a_i \leq n$)&nbsp;— the elements of the array.</p><p>The sum of $n$ across all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output a single integer&nbsp;— the <span class="tex-font-style-bf">maximum</span> number of crossings there can be if you place the wires optimally.</p>





```input1
4
7
4 1 4 6 7 7 5
2
2 1
1
1
3
2 2 2
```




```output1
6
1
0
3
```



## Note

<p>The first test case is shown in the second picture in the statement.</p><p>In the second test case, the only wiring possible has the two wires cross, so the answer is $1$.</p><p>In the third test case, the only wiring possible has one wire, so the answer is $0$.</p>
