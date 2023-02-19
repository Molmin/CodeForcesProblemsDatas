## Description

<div><p>Ori and Sein have overcome many difficult challenges. They finally lit the Shrouded Lantern and found Gumon Seal, the key to the Forlorn Ruins. When they tried to open the door to the ruins... nothing happened.</p><p>Ori was very surprised, but Sein gave the explanation quickly: clever Gumon decided to make an additional defence for the door.</p><p>There are $n$ lamps with Spirit Tree's light. Sein knows the time of turning on and off for the $i$-th lamp&nbsp;— $l_i$ and $r_i$ respectively. To open the door you have to choose $k$ lamps in such a way that there will be a moment of time when they all will be turned on.</p><p>While Sein decides which of the $k$ lamps to pick, Ori is interested: how many ways there are to pick such $k$ lamps that the door will open? It may happen that Sein may be wrong and there are no such $k$ lamps. The answer might be large, so print it modulo $998\,244\,353$.</p></div><div class="input-specification"><p>First line contains two integers $n$ and $k$ ($1 \le n \le 3 \cdot 10^5$, $1 \le k \le n$)&nbsp;— total number of lamps and the number of lamps that must be turned on simultaneously.</p><p>Next $n$ lines contain two integers $l_i$ ans $r_i$ ($1 \le l_i \le r_i \le 10^9$)&nbsp;— period of time when $i$-th lamp is turned on.</p></div><div class="output-specification"><p>Print one integer&nbsp;— the answer to the task modulo $998\,244\,353$.</p></div>

## Input

<p>First line contains two integers $n$ and $k$ ($1 \le n \le 3 \cdot 10^5$, $1 \le k \le n$)&nbsp;— total number of lamps and the number of lamps that must be turned on simultaneously.</p><p>Next $n$ lines contain two integers $l_i$ ans $r_i$ ($1 \le l_i \le r_i \le 10^9$)&nbsp;— period of time when $i$-th lamp is turned on.</p>

## Output

<p>Print one integer&nbsp;— the answer to the task modulo $998\,244\,353$.</p>





```input1
7 3
1 7
3 8
4 5
6 7
1 3
5 10
8 9
```




```input2
3 1
1 1
2 2
3 3
```




```input3
3 2
1 1
2 2
3 3
```




```input4
3 3
1 3
2 3
3 3
```




```input5
5 2
1 3
2 4
3 5
4 6
5 7
```




```output1
9
```




```output2
3
```




```output3
0
```




```output4
1
```




```output5
7
```



## Note

<p>In first test case there are nine sets of $k$ lamps: $(1, 2, 3)$, $(1, 2, 4)$, $(1, 2, 5)$, $(1, 2, 6)$, $(1, 3, 6)$, $(1, 4, 6)$, $(2, 3, 6)$, $(2, 4, 6)$, $(2, 6, 7)$.</p><p>In second test case $k=1$, so the answer is 3.</p><p>In third test case there are no such pairs of lamps.</p><p>In forth test case all lamps are turned on in a time $3$, so the answer is 1.</p><p>In fifth test case there are seven sets of $k$ lamps: $(1, 2)$, $(1, 3)$, $(2, 3)$, $(2, 4)$, $(3, 4)$, $(3, 5)$, $(4, 5)$.</p>
