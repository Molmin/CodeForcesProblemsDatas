## Description

<div><p><span class="tex-font-style-it">This problem is an extension of the problem "Wonderful Coloring - 1". It has quite many differences, so you should read this statement completely.</span></p><p>Recently, Paul and Mary have found a new favorite sequence of integers $a_1, a_2, \dots, a_n$. They want to paint it using pieces of chalk of $k$ colors. The coloring of a sequence is called <span class="tex-font-style-it">wonderful</span> if the following conditions are met:</p><ol> <li> each element of the sequence is either painted in one of $k$ colors or isn't painted; </li><li> each two elements which are painted in the same color are different (i. e. there's no two equal values painted in the same color); </li><li> let's calculate for each of $k$ colors the number of elements painted in the color — all calculated numbers must be equal; </li><li> the total number of painted elements of the sequence is the <span class="tex-font-style-bf">maximum</span> among all colorings of the sequence which meet the first three conditions. </li></ol><p>E. g. consider a sequence $a=[3, 1, 1, 1, 1, 10, 3, 10, 10, 2]$ and $k=3$. One of the wonderful colorings of the sequence is shown in the figure.</p><center> <img class="tex-graphics" src="file://U703aeKK.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">The example of a wonderful coloring of the sequence $a=[3, 1, 1, 1, 1, 10, 3, 10, 10, 2]$ and $k=3$. Note that one of the elements isn't painted.</span> </center><p>Help Paul and Mary to find a wonderful coloring of a given sequence $a$.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 10000$) — the number of test cases. Then $t$ test cases follow.</p><p>Each test case consists of two lines. The first one contains two integers $n$ and $k$ ($1 \le n \le 2\cdot10^5$, $1 \le k \le n$) — the length of a given sequence and the number of colors, respectively. The second one contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le n$).</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>Output $t$ lines, each of them must contain a description of a wonderful coloring for the corresponding test case.</p><p>Each wonderful coloring must be printed as a sequence of $n$ integers $c_1, c_2, \dots, c_n$ ($0 \le c_i \le k$) separated by spaces where</p><ul> <li> $c_i=0$, if $i$-th element isn't painted; </li><li> $c_i&gt;0$, if $i$-th element is painted in the $c_i$-th color. </li></ul><p>Remember that you need to maximize the total count of painted elements for the wonderful coloring. If there are multiple solutions, print any one.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 10000$) — the number of test cases. Then $t$ test cases follow.</p><p>Each test case consists of two lines. The first one contains two integers $n$ and $k$ ($1 \le n \le 2\cdot10^5$, $1 \le k \le n$) — the length of a given sequence and the number of colors, respectively. The second one contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le n$).</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>Output $t$ lines, each of them must contain a description of a wonderful coloring for the corresponding test case.</p><p>Each wonderful coloring must be printed as a sequence of $n$ integers $c_1, c_2, \dots, c_n$ ($0 \le c_i \le k$) separated by spaces where</p><ul> <li> $c_i=0$, if $i$-th element isn't painted; </li><li> $c_i&gt;0$, if $i$-th element is painted in the $c_i$-th color. </li></ul><p>Remember that you need to maximize the total count of painted elements for the wonderful coloring. If there are multiple solutions, print any one.</p>





```input1
6
10 3
3 1 1 1 1 10 3 10 10 2
4 4
1 1 1 1
1 1
1
13 1
3 1 4 1 5 9 2 6 5 3 5 8 9
13 2
3 1 4 1 5 9 2 6 5 3 5 8 9
13 3
3 1 4 1 5 9 2 6 5 3 5 8 9
```




```output1
1 1 0 2 3 2 2 1 3 3
4 2 1 3
1
0 0 1 1 0 1 1 1 0 1 1 1 0
2 1 2 2 1 1 1 1 2 1 0 2 2
1 1 3 2 1 3 3 1 2 2 3 2 0
```



## Note

<p>In the first test case, the answer is shown in the figure in the statement. The red color has number $1$, the blue color — $2$, the green — $3$.</p>
