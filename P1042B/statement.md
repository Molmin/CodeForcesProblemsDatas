## Description

<div><p>Berland shop sells $n$ kinds of juices. Each juice has its price $c_i$. Each juice includes some set of vitamins in it. There are three types of vitamins: vitamin "<span class="tex-font-style-tt">A</span>", vitamin "<span class="tex-font-style-tt">B</span>" and vitamin "<span class="tex-font-style-tt">C</span>". Each juice can contain one, two or all three types of vitamins in it.</p><p>Petya knows that he needs all three types of vitamins to stay healthy. What is the minimum total price of juices that Petya has to buy to obtain all three vitamins? Petya obtains some vitamin if he buys at least one juice containing it and drinks it.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ $(1 \le n \le 1\,000)$ — the number of juices.</p><p>Each of the next $n$ lines contains an integer $c_i$ $(1 \le c_i \le 100\,000)$ and a string $s_i$ — the price of the $i$-th juice and the vitamins it contains. String $s_i$ contains from $1$ to $3$ characters, and the only possible characters are "<span class="tex-font-style-tt">A</span>", "<span class="tex-font-style-tt">B</span>" and "<span class="tex-font-style-tt">C</span>". It is guaranteed that each letter appears no more than once in each string $s_i$. The order of letters in strings $s_i$ is arbitrary.</p></div><div class="output-specification"><p>Print <span class="tex-font-style-tt">-1</span> if there is no way to obtain all three vitamins. Otherwise print the minimum total price of juices that Petya has to buy to obtain all three vitamins.</p></div>

## Input

<p>The first line contains a single integer $n$ $(1 \le n \le 1\,000)$ — the number of juices.</p><p>Each of the next $n$ lines contains an integer $c_i$ $(1 \le c_i \le 100\,000)$ and a string $s_i$ — the price of the $i$-th juice and the vitamins it contains. String $s_i$ contains from $1$ to $3$ characters, and the only possible characters are "<span class="tex-font-style-tt">A</span>", "<span class="tex-font-style-tt">B</span>" and "<span class="tex-font-style-tt">C</span>". It is guaranteed that each letter appears no more than once in each string $s_i$. The order of letters in strings $s_i$ is arbitrary.</p>

## Output

<p>Print <span class="tex-font-style-tt">-1</span> if there is no way to obtain all three vitamins. Otherwise print the minimum total price of juices that Petya has to buy to obtain all three vitamins.</p>





```input1
4
5 C
6 B
16 BAC
4 A

```




```input2
2
10 AB
15 BA

```




```input3
5
10 A
9 BC
11 CA
4 A
5 B

```




```input4
6
100 A
355 BCA
150 BC
160 AC
180 B
190 CA

```




```input5
2
5 BA
11 CB

```




```output1
15

```




```output2
-1

```




```output3
13

```




```output4
250

```




```output5
16

```



## Note

<p>In the first example Petya buys the first, the second and the fourth juice. He spends $5 + 6 + 4 = 15$ and obtains all three vitamins. He can also buy just the third juice and obtain three vitamins, but its cost is $16$, which isn't optimal.</p><p>In the second example Petya can't obtain all three vitamins, as no juice contains vitamin "<span class="tex-font-style-tt">C</span>".</p>
