## Description

<div><p>Acingel is a small town. There was only one doctor here&nbsp;— Miss Ada. She was very friendly and nobody has ever said something bad about her, so who could've expected that Ada will be found dead in her house? Mr Gawry, world-famous detective, is appointed to find the criminal. He asked $m$ neighbours of Ada about clients who have visited her in that unlucky day. Let's number the clients from $1$ to $n$. Each neighbour's testimony is a permutation of these numbers, which describes the order in which clients have been seen by the asked neighbour.</p><p>However, some facts are very suspicious&nbsp;– how it is that, according to some of given permutations, some client has been seen in the morning, while in others he has been seen in the evening? "In the morning some of neighbours must have been sleeping!"&nbsp;— thinks Gawry&nbsp;— "and in the evening there's been too dark to see somebody's face...". Now he wants to delete some prefix and some suffix (both prefix and suffix can be empty) in each permutation, so that they'll be non-empty and equal to each other after that&nbsp;— some of the potential criminals may disappear, but the testimony won't stand in contradiction to each other.</p><p>In how many ways he can do it? Two ways are called different if the remaining common part is different.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \le n \le 100\,000$, $1 \le m \le 10$)&nbsp;— the number of suspects and the number of asked neighbors.</p><p>Each of the next $m$ lines contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le n$). It is guaranteed that these integers form a correct permutation (that is, each number from $1$ to $n$ appears exactly once).</p></div><div class="output-specification"><p>Output a single integer denoting the number of ways to delete some prefix and some suffix of each permutation (possibly empty), such that the remaining parts will be equal and non-empty.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \le n \le 100\,000$, $1 \le m \le 10$)&nbsp;— the number of suspects and the number of asked neighbors.</p><p>Each of the next $m$ lines contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le n$). It is guaranteed that these integers form a correct permutation (that is, each number from $1$ to $n$ appears exactly once).</p>

## Output

<p>Output a single integer denoting the number of ways to delete some prefix and some suffix of each permutation (possibly empty), such that the remaining parts will be equal and non-empty.</p>





```input1
3 2
1 2 3
2 3 1

```




```input2
5 6
1 2 3 4 5
2 3 1 4 5
3 4 5 1 2
3 5 4 2 1
2 3 5 4 1
1 2 3 4 5

```




```input3
2 2
1 2
2 1

```




```output1
4

```




```output2
5

```




```output3
2

```



## Note

<p>In the first example, all possible common parts are $[1]$, $[2]$, $[3]$ and $[2, 3]$.</p><p>In the second and third examples, you can only leave common parts of length $1$.</p>
