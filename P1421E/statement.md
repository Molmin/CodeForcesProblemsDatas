## Description

<div><p>While playing yet another strategy game, Mans has recruited $n$ <a href="https://www.youtube.com/watch?v=5sGOwFVUU0I">Swedish heroes</a>, whose powers which can be represented as an array $a$.</p><p>Unfortunately, not all of those mighty heroes were created as capable as he wanted, so that he decided to do something about it. In order to accomplish his goal, he can pick two consecutive heroes, with powers $a_i$ and $a_{i+1}$, remove them and insert a hero with power $-(a_i+a_{i+1})$ back in the same position. </p><p>For example if the array contains the elements $[5, 6, 7, 8]$, he can pick $6$ and $7$ and get $[5, -(6+7), 8] = [5, -13, 8]$.</p><p>After he will perform this operation $n-1$ times, Mans will end up having only one hero. He wants his power to be as big as possible. What's the largest possible power he can achieve?</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 200000$).</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($-10^9 \le a_i \le 10^9$)&nbsp;— powers of the heroes.</p></div><div class="output-specification"><p>Print the largest possible power he can achieve after $n-1$ operations.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 200000$).</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($-10^9 \le a_i \le 10^9$)&nbsp;— powers of the heroes.</p>

## Output

<p>Print the largest possible power he can achieve after $n-1$ operations.</p>





```input1
4
5 6 7 8
```




```input2
5
4 -5 9 -2 1
```




```output1
26
```




```output2
15
```



## Note

<p>Suitable list of operations for the first sample:</p><p>$[5, 6, 7, 8] \rightarrow [-11, 7, 8] \rightarrow [-11, -15] \rightarrow [26]$</p>
