## Description

<div><p>One way to create a task is to learn from math. You can generate some random math statement or modify some theorems to get something new and build a new task from that.</p><p>For example, there is a statement called the "Goldbach's conjecture". It says: "each even number no less than four can be expressed as the sum of two primes". Let's modify it. How about a statement like that: "each integer no less than 12 can be expressed as the sum of two composite numbers." Not like the Goldbach's conjecture, I can prove this theorem.</p><p>You are given an integer <span class="tex-span"><i>n</i></span> no less than 12, express it as a sum of two composite numbers.</p></div><div class="input-specification"><p>The only line contains an integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(12 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>)</span>.</p></div><div class="output-specification"><p>Output two composite integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> <span class="tex-span">(1 &lt; <i>x</i>, <i>y</i> &lt; <i>n</i>)</span> such that <span class="tex-span"><i>x</i> + <i>y</i> = <i>n</i></span>. If there are multiple solutions, you can output any of them.</p></div>

## Input

<p>The only line contains an integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(12 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>)</span>.</p>

## Output

<p>Output two composite integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> <span class="tex-span">(1 &lt; <i>x</i>, <i>y</i> &lt; <i>n</i>)</span> such that <span class="tex-span"><i>x</i> + <i>y</i> = <i>n</i></span>. If there are multiple solutions, you can output any of them.</p>





```input1
12

```




```input2
15

```




```input3
23

```




```input4
1000000

```




```output1
4 8

```




```output2
6 9

```




```output3
8 15

```




```output4
500000 500000

```



## Note

<p>In the first example, 12 = 4 + 8 and both 4, 8 are composite numbers. You can output "6 6" or "8 4" as well.</p><p>In the second example, 15 = 6 + 9. Note that you can't output "1 14" because 1 is not a composite number.</p>
