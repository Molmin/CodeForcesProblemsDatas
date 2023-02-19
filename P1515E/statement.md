## Description

<div><p>There are $n$ computers in a row, all originally off, and Phoenix wants to turn all of them on. He will manually turn on computers one at a time. At any point, if computer $i-1$ and computer $i+1$ are both on, computer $i$ $(2 \le i \le n-1)$ will turn on automatically if it is not already on. Note that Phoenix cannot manually turn on a computer that already turned on automatically.</p><p>If we only consider the sequence of computers that Phoenix turns on manually, how many ways can he turn on all the computers? Two sequences are distinct if either the set of computers turned on manually is distinct, or the order of computers turned on manually is distinct. Since this number may be large, please print it modulo $M$.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $M$ ($3 \le n \le 400$; $10^8 \le M \le 10^9$)&nbsp;— the number of computers and the modulo. It is guaranteed that $M$ is prime.</p></div><div class="output-specification"><p>Print one integer&nbsp;— the number of ways to turn on the computers modulo $M$.</p></div>

## Input

<p>The first line contains two integers $n$ and $M$ ($3 \le n \le 400$; $10^8 \le M \le 10^9$)&nbsp;— the number of computers and the modulo. It is guaranteed that $M$ is prime.</p>

## Output

<p>Print one integer&nbsp;— the number of ways to turn on the computers modulo $M$.</p>





```input1
3 100000007
```




```input2
4 100000007
```




```input3
400 234567899
```




```output1
6
```




```output2
20
```




```output3
20914007
```



## Note

<p>In the first example, these are the $6$ orders in which Phoenix can turn on all computers: </p><ul> <li> $[1,3]$. Turn on computer $1$, then $3$. Note that computer $2$ turns on automatically after computer $3$ is turned on manually, but we only consider the sequence of computers that are turned on manually. </li><li> $[3,1]$. Turn on computer $3$, then $1$. </li><li> $[1,2,3]$. Turn on computer $1$, $2$, then $3$. </li><li> $[2,1,3]$ </li><li> $[2,3,1]$ </li><li> $[3,2,1]$ </li></ul>
