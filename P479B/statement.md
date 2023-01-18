## Description

<div><p>As you know, all the kids in Berland love playing with cubes. Little Petya has <span class="tex-span"><i>n</i></span> towers consisting of cubes of the same size. Tower with number <span class="tex-span"><i>i</i></span> consists of <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> cubes stacked one on top of the other. Petya defines the <span class="tex-font-style-it">instability</span> of a set of towers as a value equal to the difference between the heights of the highest and the lowest of the towers. For example, if Petya built five cube towers with heights (8, 3, 2, 6, 3), the instability of this set is equal to 6 (the highest tower has height 8, the lowest one has height 2). </p><p>The boy wants the instability of his set of towers to be as low as possible. All he can do is to perform the following operation several times: take the top cube from some tower and put it on top of some other tower of his set. Please note that Petya would never put the cube on the same tower from which it was removed because he thinks it's a waste of time. </p><p>Before going to school, the boy will have time to perform no more than <span class="tex-span"><i>k</i></span> such operations. Petya does not want to be late for class, so you have to help him accomplish this task.</p></div><div class="input-specification"><p>The first line contains two space-separated positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 1000</span>) — the number of towers in the given set and the maximum number of operations Petya can perform. The second line contains <span class="tex-span"><i>n</i></span> space-separated positive integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>) — the towers' initial heights.</p></div><div class="output-specification"><p>In the first line print two space-separated non-negative integers <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span"><i>m</i> ≤ <i>k</i></span>). The first number is the value of the minimum possible instability that can be obtained after performing at most <span class="tex-span"><i>k</i></span> operations, the second number is the number of operations needed for that.</p><p>In the next <span class="tex-span"><i>m</i></span> lines print the description of each operation as two positive integers <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span>, each of them lies within limits from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. They represent that Petya took the top cube from the <span class="tex-span"><i>i</i></span>-th tower and put in on the <span class="tex-span"><i>j</i></span>-th one (<span class="tex-span"><i>i</i> ≠ <i>j</i></span>). Note that in the process of performing operations the heights of some towers can become equal to zero.</p><p>If there are multiple correct sequences at which the minimum possible instability is achieved, you are allowed to print any of them.</p></div>

## Input

<p>The first line contains two space-separated positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 1000</span>) — the number of towers in the given set and the maximum number of operations Petya can perform. The second line contains <span class="tex-span"><i>n</i></span> space-separated positive integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>) — the towers' initial heights.</p>

## Output

<p>In the first line print two space-separated non-negative integers <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span"><i>m</i> ≤ <i>k</i></span>). The first number is the value of the minimum possible instability that can be obtained after performing at most <span class="tex-span"><i>k</i></span> operations, the second number is the number of operations needed for that.</p><p>In the next <span class="tex-span"><i>m</i></span> lines print the description of each operation as two positive integers <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span>, each of them lies within limits from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. They represent that Petya took the top cube from the <span class="tex-span"><i>i</i></span>-th tower and put in on the <span class="tex-span"><i>j</i></span>-th one (<span class="tex-span"><i>i</i> ≠ <i>j</i></span>). Note that in the process of performing operations the heights of some towers can become equal to zero.</p><p>If there are multiple correct sequences at which the minimum possible instability is achieved, you are allowed to print any of them.</p>





```input1
3 2
5 8 5

```




```input2
3 4
2 2 4

```




```input3
5 3
8 3 2 6 3

```




```output1
0 2
2 1
2 3

```




```output2
1 1
3 2

```




```output3
3 3
1 3
1 2
1 3

```



## Note

<p>In the first sample you need to move the cubes two times, from the second tower to the third one and from the second one to the first one. Then the heights of the towers are all the same and equal to 6.</p>
