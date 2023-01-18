## Description

<div><p>You are given a positive integer $n$ greater or equal to $2$. For every pair of integers $a$ and $b$ ($2 \le |a|, |b| \le n$), you can transform $a$ into $b$ if and only if there exists an integer $x$ such that $1 &lt; |x|$ and ($a \cdot x = b$ or $b \cdot x = a$), where $|x|$ denotes the absolute value of $x$.</p><p>After such a transformation, your score increases by $|x|$ points and you are <span class="tex-font-style-bf">not allowed</span> to transform $a$ into $b$ nor $b$ into $a$ anymore.</p><p>Initially, you have a score of $0$. You can start at any integer and transform it as many times as you like. What is the maximum score you can achieve?</p></div><div class="input-specification"><p>A single line contains a single integer $n$ ($2 \le n \le 100\,000$)&nbsp;— the given integer described above.</p></div><div class="output-specification"><p>Print an only integer&nbsp;— the maximum score that can be achieved with the transformations. If it is not possible to perform even a single transformation for all possible starting integers, print $0$.</p></div>

## Input

<p>A single line contains a single integer $n$ ($2 \le n \le 100\,000$)&nbsp;— the given integer described above.</p>

## Output

<p>Print an only integer&nbsp;— the maximum score that can be achieved with the transformations. If it is not possible to perform even a single transformation for all possible starting integers, print $0$.</p>





```input1
4

```




```input2
6

```




```input3
2

```




```output1
8
```




```output2
28
```




```output3
0
```



## Note

<p>In the first example, the transformations are $2 \rightarrow 4 \rightarrow (-2) \rightarrow (-4) \rightarrow 2$.</p><p>In the third example, it is impossible to perform even a single transformation.</p>
