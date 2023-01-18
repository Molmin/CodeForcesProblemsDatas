## Description

<div><p>In the Isle of Guernsey there are <span class="tex-span"><i>n</i></span> different types of coins. For each <span class="tex-span"><i>i</i></span> <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>n</i>)</span>, coin of type <span class="tex-span"><i>i</i></span> is worth <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> cents. It is possible that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = <i>a</i><sub class="lower-index"><i>j</i></sub></span> for some <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> <span class="tex-span">(<i>i</i> ≠ <i>j</i>)</span>. </p><p>Bessie has some set of these coins totaling <span class="tex-span"><i>t</i></span> cents. She tells Jessie <span class="tex-span"><i>q</i></span> pairs of integers. For each <span class="tex-span"><i>i</i></span> <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>q</i>)</span>, the pair <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub></span> tells Jessie that Bessie has a strictly greater number of coins of type <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> than coins of type <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>. It is known that all <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> are distinct and all <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> are distinct. </p><p>Help Jessie find the number of possible combinations of coins Bessie could have. Two combinations are considered different if there is some <span class="tex-span"><i>i</i></span> <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>n</i>)</span>, such that the number of coins Bessie has of type <span class="tex-span"><i>i</i></span> is different in the two combinations. Since the answer can be very large, output it modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>. </p><p>If there are no possible combinations of coins totaling <span class="tex-span"><i>t</i></span> cents that satisfy Bessie's conditions, output 0.</p></div><div class="input-specification"><p>The first line contains three space-separated integers, <span class="tex-span"><i>n</i>, <i>q</i></span> and <span class="tex-span"><i>t</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 300;&nbsp;0 ≤ <i>q</i> ≤ <i>n</i>;&nbsp;1 ≤ <i>t</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The second line contains <span class="tex-span"><i>n</i></span> space separated integers, <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span>. The next <span class="tex-span"><i>q</i></span> lines each contain two distinct space-separated integers, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>b</i><sub class="lower-index"><i>i</i></sub> ≠ <i>c</i><sub class="lower-index"><i>i</i></sub>)</span>.</p><p>It's guaranteed that all <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> are distinct and all <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> are distinct.</p></div><div class="output-specification"><p>A single integer, the number of valid coin combinations that Bessie could have, modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>The first line contains three space-separated integers, <span class="tex-span"><i>n</i>, <i>q</i></span> and <span class="tex-span"><i>t</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 300;&nbsp;0 ≤ <i>q</i> ≤ <i>n</i>;&nbsp;1 ≤ <i>t</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The second line contains <span class="tex-span"><i>n</i></span> space separated integers, <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span>. The next <span class="tex-span"><i>q</i></span> lines each contain two distinct space-separated integers, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>b</i><sub class="lower-index"><i>i</i></sub> ≠ <i>c</i><sub class="lower-index"><i>i</i></sub>)</span>.</p><p>It's guaranteed that all <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> are distinct and all <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> are distinct.</p>

## Output

<p>A single integer, the number of valid coin combinations that Bessie could have, modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
4 2 17
3 1 2 5
4 2
3 4

```




```input2
3 2 6
3 1 1
1 2
2 3

```




```input3
3 2 10
1 2 3
1 2
2 1

```




```output1
3

```




```output2
0

```




```output3
0

```



## Note

<p>For the first sample, the following 3 combinations give a total of 17 cents and satisfy the given conditions: <span class="tex-span">{0&nbsp;<i>of</i>&nbsp;<i>type</i>&nbsp;1, 1&nbsp;<i>of</i>&nbsp;<i>type</i>&nbsp;2, 3&nbsp;<i>of</i>&nbsp;<i>type</i>&nbsp;3, 2&nbsp;<i>of</i>&nbsp;<i>type</i>&nbsp;4}, {0, 0, 6, 1}, {2, 0, 3, 1}</span>.</p><p>No other combinations exist. Note that even though 4 occurs in both <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub>, </span> the problem conditions are still satisfied because all <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> are distinct and all <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> are distinct.</p>
