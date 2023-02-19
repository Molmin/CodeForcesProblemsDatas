## Description

<div><p>Polycarp has a favorite sequence $a[1 \dots n]$ consisting of $n$ integers. He wrote it out on the whiteboard as follows:</p><ul> <li> he wrote the number $a_1$ to the left side (at the beginning of the whiteboard); </li><li> he wrote the number $a_2$ to the right side (at the end of the whiteboard); </li><li> then as far to the left as possible (but to the right from $a_1$), he wrote the number $a_3$; </li><li> then as far to the right as possible (but to the left from $a_2$), he wrote the number $a_4$; </li><li> Polycarp continued to act as well, until he wrote out the entire sequence on the whiteboard. </li></ul><center> <img class="tex-graphics" src="file://Z4lChWxy.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">The beginning of the result looks like this (of course, if $n \ge 4$).</span> </center><p>For example, if $n=7$ and $a=[3, 1, 4, 1, 5, 9, 2]$, then Polycarp will write a sequence on the whiteboard $[3, 4, 5, 2, 9, 1, 1]$.</p><p>You saw the sequence written on the whiteboard and now you want to restore Polycarp's favorite sequence.</p></div><div class="input-specification"><p>The first line contains a single positive integer $t$ ($1 \le t \le 300$)&nbsp;— the number of test cases in the test. Then $t$ test cases follow.</p><p>The first line of each test case contains an integer $n$ ($1 \le n \le 300$)&nbsp;— the length of the sequence written on the whiteboard.</p><p>The next line contains $n$ integers $b_1, b_2,\ldots, b_n$ ($1 \le b_i \le 10^9$)&nbsp;— the sequence written on the whiteboard.</p></div><div class="output-specification"><p>Output $t$ answers to the test cases. Each answer&nbsp;— is a sequence $a$ that Polycarp wrote out on the whiteboard.</p></div>

## Input

<p>The first line contains a single positive integer $t$ ($1 \le t \le 300$)&nbsp;— the number of test cases in the test. Then $t$ test cases follow.</p><p>The first line of each test case contains an integer $n$ ($1 \le n \le 300$)&nbsp;— the length of the sequence written on the whiteboard.</p><p>The next line contains $n$ integers $b_1, b_2,\ldots, b_n$ ($1 \le b_i \le 10^9$)&nbsp;— the sequence written on the whiteboard.</p>

## Output

<p>Output $t$ answers to the test cases. Each answer&nbsp;— is a sequence $a$ that Polycarp wrote out on the whiteboard.</p>





```input1
6
7
3 4 5 2 9 1 1
4
9 2 7 1
11
8 4 3 1 2 7 8 7 9 4 2
1
42
2
11 7
8
1 1 1 1 1 1 1 1
```




```output1
3 1 4 1 5 9 2 
9 1 2 7 
8 2 4 4 3 9 1 7 2 8 7 
42 
11 7 
1 1 1 1 1 1 1 1
```



## Note

<p>In the first test case, the sequence $a$ matches the sequence from the statement. The whiteboard states after each step look like this:</p><p>$[3] \Rightarrow [3, 1] \Rightarrow [3, 4, 1] \Rightarrow [3, 4, 1, 1] \Rightarrow [3, 4, 5, 1, 1] \Rightarrow [3, 4, 5, 9, 1, 1] \Rightarrow [3, 4, 5, 2, 9, 1, 1]$.</p>
