## Description

<div><p>Little girl Tanya is learning how to decrease a number by one, but she does it wrong with a number consisting of two or more digits. Tanya subtracts one from a number by the following algorithm:</p><ul> <li> if the last digit of the number is non-zero, she decreases the number by one; </li><li> if the last digit of the number is zero, she divides the number by 10 (i.e. removes the last digit). </li></ul><p>You are given an integer number $n$. Tanya will subtract one from it $k$ times. Your task is to print the result after all $k$ subtractions.</p><p>It is guaranteed that the result will be positive integer number.</p></div><div class="input-specification"><p>The first line of the input contains two integer numbers $n$ and $k$ ($2 \le n \le 10^9$, $1 \le k \le 50$) — the number from which Tanya will subtract and the number of subtractions correspondingly.</p></div><div class="output-specification"><p>Print one integer number — the result of the decreasing $n$ by one $k$ times.</p><p>It is guaranteed that the result will be positive integer number. </p></div>

## Input

<p>The first line of the input contains two integer numbers $n$ and $k$ ($2 \le n \le 10^9$, $1 \le k \le 50$) — the number from which Tanya will subtract and the number of subtractions correspondingly.</p>

## Output

<p>Print one integer number — the result of the decreasing $n$ by one $k$ times.</p><p>It is guaranteed that the result will be positive integer number. </p>





```input1
512 4

```




```input2
1000000000 9

```




```output1
50

```




```output2
1

```



## Note

<p>The first example corresponds to the following sequence: $512 \rightarrow 511 \rightarrow 510 \rightarrow 51 \rightarrow 50$.</p>
