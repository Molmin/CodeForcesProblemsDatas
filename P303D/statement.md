## Description

<div><p>Bike is a smart boy who loves math very much. He invented a number called "Rotatable Number" inspired by <span class="tex-span">142857</span>. </p><p>As you can see, <span class="tex-span">142857</span> is a magic number because any of its rotatings can be got by multiplying that number by <span class="tex-span">1, 2, ..., 6</span> (numbers from one to number's length). Rotating a number means putting its last several digit into first. For example, by rotating number <span class="tex-span">12345</span> you can obtain any numbers: <span class="tex-span">12345, 51234, 45123, 34512, 23451</span>. It's worth mentioning that <span class="tex-font-style-bf">leading-zeroes</span> are allowed. So both <span class="tex-span">4500123</span> and <span class="tex-span">0123450</span> can be obtained by rotating <span class="tex-span">0012345</span>. You can see why <span class="tex-span">142857</span> satisfies the condition. All of the <span class="tex-span">6</span> equations are under base <span class="tex-span">10</span>.</p><ul> <li> <span class="tex-span">142857·1 = 142857</span>; </li><li> <span class="tex-span">142857·2 = 285714</span>; </li><li> <span class="tex-span">142857·3 = 428571</span>; </li><li> <span class="tex-span">142857·4 = 571428</span>; </li><li> <span class="tex-span">142857·5 = 714285</span>; </li><li> <span class="tex-span">142857·6 = 857142</span>. </li></ul><p>Now, Bike has a problem. He extends "Rotatable Number" under any base <span class="tex-span"><i>b</i></span>. As is mentioned above, <span class="tex-span">142857</span> is a "Rotatable Number" under base <span class="tex-span">10</span>. Another example is <span class="tex-span">0011</span> under base 2. All of the <span class="tex-span">4</span> equations are under base <span class="tex-span">2</span>.</p><ul> <li> <span class="tex-span">0011·1 = 0011</span>; </li><li> <span class="tex-span">0011·10 = 0110</span>; </li><li> <span class="tex-span">0011·11 = 1001</span>; </li><li> <span class="tex-span">0011·100 = 1100</span>. </li></ul><p>So, he wants to find the largest <span class="tex-span"><i>b</i></span> <span class="tex-span">(1 &lt; <i>b</i> &lt; <i>x</i>)</span> so that there is a <span class="tex-font-style-bf">positive</span> "Rotatable Number" (leading-zeroes allowed) of length <span class="tex-span"><i>n</i></span> under base <span class="tex-span"><i>b</i></span>.</p><p>Note that any time you multiply a rotatable number by numbers from 1 to its length you should get a rotating of that number.</p></div><div class="input-specification"><p>The only line contains two space-separated integers <span class="tex-span"><i>n</i>, <i>x</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">6</sup>, 2 ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup>)</span>. </p></div><div class="output-specification"><p>Print a single integer — the largest <span class="tex-span"><i>b</i></span> you found. If no such <span class="tex-span"><i>b</i></span> exists, print <span class="tex-font-style-tt">-1</span> instead. </p></div>

## Input

<p>The only line contains two space-separated integers <span class="tex-span"><i>n</i>, <i>x</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">6</sup>, 2 ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup>)</span>. </p>

## Output

<p>Print a single integer — the largest <span class="tex-span"><i>b</i></span> you found. If no such <span class="tex-span"><i>b</i></span> exists, print <span class="tex-font-style-tt">-1</span> instead. </p>





```input1
6 11

```




```input2
5 8

```




```output1
10

```




```output2
-1

```


