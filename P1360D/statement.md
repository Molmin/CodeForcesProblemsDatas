## Description

<div><p>Polycarp wants to buy <span class="tex-font-style-bf">exactly</span> $n$ shovels. The shop sells packages with shovels. The store has $k$ types of packages: the package of the $i$-th type consists of exactly $i$ shovels ($1 \le i \le k$). The store has an infinite number of packages of each type.</p><p>Polycarp wants to choose <span class="tex-font-style-bf">one</span> type of packages and then buy several (one or more) packages of this type. What is the smallest number of packages Polycarp will have to buy to get exactly $n$ shovels?</p><p>For example, if $n=8$ and $k=7$, then Polycarp will buy $2$ packages of $4$ shovels.</p><p>Help Polycarp find the minimum number of packages that he needs to buy, given that he: </p><ul> <li> will buy exactly $n$ shovels in total; </li><li> the sizes of <span class="tex-font-style-bf">all</span> packages he will buy are all the same and the number of shovels in each package is an integer from $1$ to $k$, inclusive. </li></ul></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 100$)&nbsp;— the number of test cases in the input. Then, $t$ test cases follow, one per line.</p><p>Each test case consists of two positive integers $n$ ($1 \le n \le 10^9$) and $k$ ($1 \le k \le 10^9$)&nbsp;— the number of shovels and the number of types of packages.</p></div><div class="output-specification"><p>Print $t$ answers to the test cases. Each answer is a positive integer&nbsp;— the minimum number of packages.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 100$)&nbsp;— the number of test cases in the input. Then, $t$ test cases follow, one per line.</p><p>Each test case consists of two positive integers $n$ ($1 \le n \le 10^9$) and $k$ ($1 \le k \le 10^9$)&nbsp;— the number of shovels and the number of types of packages.</p>

## Output

<p>Print $t$ answers to the test cases. Each answer is a positive integer&nbsp;— the minimum number of packages.</p>





```input1
5
8 7
8 1
6 10
999999733 999999732
999999733 999999733
```




```output1
2
8
1
999999733
1
```



## Note

<p>The answer to the first test case was explained in the statement.</p><p>In the second test case, there is only one way to buy $8$ shovels&nbsp;— $8$ packages of one shovel.</p><p>In the third test case, you need to buy a $1$ package of $6$ shovels.</p>
