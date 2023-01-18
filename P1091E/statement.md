## Description

<div><p>Bob is an active user of the social network Faithbug. On this network, people are able to engage in a mutual friendship. That is, if $a$ is a friend of $b$, then $b$ is also a friend of $a$. Each user thus has a non-negative amount of friends.</p><p>This morning, somebody anonymously sent Bob the following link: <a href="https://en.wikipedia.org/wiki/Graph_realization_problem">graph realization problem</a> and Bob wants to know who that was. In order to do that, he first needs to know how the social network looks like. He investigated the profile of every other person on the network and noted down the number of his friends. However, he neglected to note down the number of his friends. Help him find out how many friends he has. Since there may be many possible answers, print <span class="tex-font-style-bf">all</span> of them.</p></div><div class="input-specification"><p>The first line contains one integer $n$&nbsp;($1 \leq n \leq 5 \cdot 10^5$), the number of people on the network <span class="tex-font-style-bf">excluding</span> Bob. </p><p>The second line contains $n$ numbers $a_1,a_2, \dots, a_n$&nbsp;($0 \leq a_i \leq n$), with $a_i$ being the number of people that person $i$ is a friend of.</p></div><div class="output-specification"><p>Print all possible values of $a_{n+1}$&nbsp;— the amount of people that Bob can be friend of, <span class="tex-font-style-bf">in increasing order</span>.</p><p>If no solution exists, output $-1$.</p></div>

## Input

<p>The first line contains one integer $n$&nbsp;($1 \leq n \leq 5 \cdot 10^5$), the number of people on the network <span class="tex-font-style-bf">excluding</span> Bob. </p><p>The second line contains $n$ numbers $a_1,a_2, \dots, a_n$&nbsp;($0 \leq a_i \leq n$), with $a_i$ being the number of people that person $i$ is a friend of.</p>

## Output

<p>Print all possible values of $a_{n+1}$&nbsp;— the amount of people that Bob can be friend of, <span class="tex-font-style-bf">in increasing order</span>.</p><p>If no solution exists, output $-1$.</p>





```input1
3
3 3 3

```




```input2
4
1 1 1 1

```




```input3
2
0 2

```




```input4
35
21 26 18 4 28 2 15 13 16 25 6 32 11 5 31 17 9 3 24 33 14 27 29 1 20 4 12 7 10 30 34 8 19 23 22

```




```output1
3 

```




```output2
0 2 4 

```




```output3
-1

```




```output4
13 15 17 19 21 

```



## Note

<p>In the first test case, the only solution is that everyone is friends with everyone. That is why Bob should have $3$ friends.</p><p>In the second test case, there are three possible solutions (apart from symmetries): </p><ul> <li> $a$ is friend of $b$, $c$ is friend of $d$, and Bob has no friends, or </li><li> $a$ is a friend of $b$ and both $c$ and $d$ are friends with Bob, or </li><li> Bob is friends of everyone. </li></ul><p>The third case is impossible to solve, as the second person needs to be a friend with everybody, but the first one is a complete stranger.</p>
