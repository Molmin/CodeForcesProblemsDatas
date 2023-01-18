## Description

<div><p>There are $n$ benches in the Berland Central park. It is known that $a_i$ people are currently sitting on the $i$-th bench. Another $m$ people are coming to the park and each of them is going to have a seat on some bench out of $n$ available.</p><p>Let $k$ be the maximum number of people sitting on one bench after additional $m$ people came to the park. Calculate the minimum possible $k$ and the maximum possible $k$.</p><p>Nobody leaves the taken seat during the whole process.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ $(1 \le n \le 100)$ — the number of benches in the park.</p><p>The second line contains a single integer $m$ $(1 \le m \le 10\,000)$ — the number of people additionally coming to the park.</p><p>Each of the next $n$ lines contains a single integer $a_i$ $(1 \le a_i \le 100)$ — the initial number of people on the $i$-th bench.</p></div><div class="output-specification"><p>Print the minimum possible $k$ and the maximum possible $k$, where $k$ is the maximum number of people sitting on one bench after additional $m$ people came to the park.</p></div>

## Input

<p>The first line contains a single integer $n$ $(1 \le n \le 100)$ — the number of benches in the park.</p><p>The second line contains a single integer $m$ $(1 \le m \le 10\,000)$ — the number of people additionally coming to the park.</p><p>Each of the next $n$ lines contains a single integer $a_i$ $(1 \le a_i \le 100)$ — the initial number of people on the $i$-th bench.</p>

## Output

<p>Print the minimum possible $k$ and the maximum possible $k$, where $k$ is the maximum number of people sitting on one bench after additional $m$ people came to the park.</p>





```input1
4
6
1
1
1
1

```




```input2
1
10
5

```




```input3
3
6
1
6
5

```




```input4
3
7
1
6
5

```




```output1
3 7

```




```output2
15 15

```




```output3
6 12

```




```output4
7 13

```



## Note

<p>In the first example, each of four benches is occupied by a single person. The minimum $k$ is $3$. For example, it is possible to achieve if two newcomers occupy the first bench, one occupies the second bench, one occupies the third bench, and two remaining — the fourth bench. The maximum $k$ is $7$. That requires all six new people to occupy the same bench.</p><p>The second example has its minimum $k$ equal to $15$ and maximum $k$ equal to $15$, as there is just a single bench in the park and all $10$ people will occupy it.</p>
