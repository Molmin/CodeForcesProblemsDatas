## Description

<div><p>JATC's math teacher always gives the class some interesting math problems so that they don't get bored. Today the problem is as follows. Given an integer $n$, you can perform the following operations zero or more times:</p><ul> <li> <span class="tex-font-style-tt">mul</span> $x$: multiplies $n$ by $x$ (where $x$ is an arbitrary positive integer). </li><li> <span class="tex-font-style-tt">sqrt</span>: replaces $n$ with $\sqrt{n}$ (to apply this operation, $\sqrt{n}$ must be an integer). </li></ul><p>You can perform these operations as many times as you like. What is the minimum value of $n$, that can be achieved and what is the minimum number of operations, to achieve that minimum value?</p><p>Apparently, no one in the class knows the answer to this problem, maybe you can help them?</p></div><div class="input-specification"><p>The only line of the input contains a single integer $n$ ($1 \le n \le 10^6$)&nbsp;— the initial number.</p></div><div class="output-specification"><p>Print two integers: the minimum integer $n$ that can be achieved using the described operations and the minimum number of operations required.</p></div>

## Input

<p>The only line of the input contains a single integer $n$ ($1 \le n \le 10^6$)&nbsp;— the initial number.</p>

## Output

<p>Print two integers: the minimum integer $n$ that can be achieved using the described operations and the minimum number of operations required.</p>





```input1
20

```




```input2
5184

```




```output1
10 2
```




```output2
6 4
```



## Note

<p>In the first example, you can apply the operation <span class="tex-font-style-tt">mul</span> $5$ to get $100$ and then <span class="tex-font-style-tt">sqrt</span> to get $10$.</p><p>In the second example, you can first apply <span class="tex-font-style-tt">sqrt</span> to get $72$, then <span class="tex-font-style-tt">mul</span> $18$ to get $1296$ and finally two more <span class="tex-font-style-tt">sqrt</span> and you get $6$.</p><p>Note, that even if the initial value of $n$ is less or equal $10^6$, it can still become greater than $10^6$ after applying one or more operations.</p>
