## Description

<div><p>There are a lot of things which could be cut&nbsp;— trees, paper, "the rope". In this problem you are going to cut a sequence of integers.</p><p>There is a sequence of integers, which contains the equal number of even and odd numbers. Given a limited budget, you need to make maximum possible number of cuts such that each resulting segment will have the same number of odd and even integers.</p><p>Cuts separate a sequence to continuous (contiguous) segments. You may think about each cut as a break between two adjacent elements in a sequence. So after cutting each element belongs to exactly one segment. Say, $[4, 1, 2, 3, 4, 5, 4, 4, 5, 5]$ $\to$ two cuts $\to$ $[4, 1 | 2, 3, 4, 5 | 4, 4, 5, 5]$. On each segment the number of even elements should be equal to the number of odd elements.</p><p>The cost of the cut between $x$ and $y$ numbers is $|x - y|$ bitcoins. Find the maximum possible number of cuts that can be made while spending no more than $B$ bitcoins.</p></div><div class="input-specification"><p>First line of the input contains an integer $n$ ($2 \le n \le 100$) and an integer $B$ ($1 \le B \le 100$)&nbsp;— the number of elements in the sequence and the number of bitcoins you have.</p><p>Second line contains $n$ integers: $a_1$, $a_2$, ..., $a_n$ ($1 \le a_i \le 100$)&nbsp;— elements of the sequence, which contains the equal number of even and odd numbers</p></div><div class="output-specification"><p>Print the maximum possible number of cuts which can be made while spending no more than $B$ bitcoins.</p></div>

## Input

<p>First line of the input contains an integer $n$ ($2 \le n \le 100$) and an integer $B$ ($1 \le B \le 100$)&nbsp;— the number of elements in the sequence and the number of bitcoins you have.</p><p>Second line contains $n$ integers: $a_1$, $a_2$, ..., $a_n$ ($1 \le a_i \le 100$)&nbsp;— elements of the sequence, which contains the equal number of even and odd numbers</p>

## Output

<p>Print the maximum possible number of cuts which can be made while spending no more than $B$ bitcoins.</p>





```input1
6 4
1 2 5 10 15 20

```




```input2
4 10
1 3 2 4

```




```input3
6 100
1 2 3 4 5 6

```




```output1
1

```




```output2
0

```




```output3
2

```



## Note

<p>In the first sample the optimal answer is to split sequence between $2$ and $5$. Price of this cut is equal to $3$ bitcoins.</p><p>In the second sample it is not possible to make even one cut even with unlimited number of bitcoins.</p><p>In the third sample the sequence should be cut between $2$ and $3$, and between $4$ and $5$. The total price of the cuts is $1 + 1 = 2$ bitcoins.</p>
