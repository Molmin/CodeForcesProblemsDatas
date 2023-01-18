## Description

<div><p>Alyona's mother wants to present an array of <span class="tex-span"><i>n</i></span> non-negative integers to Alyona. The array should be special. </p><p>Alyona is a capricious girl so after she gets the array, she inspects <span class="tex-span"><i>m</i></span> of its subarrays. Subarray is a set of some subsequent elements of the array. The <span class="tex-span"><i>i</i></span>-th subarray is described with two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>, and its elements are <span class="tex-span"><i>a</i>[<i>l</i><sub class="lower-index"><i>i</i></sub>], <i>a</i>[<i>l</i><sub class="lower-index"><i>i</i></sub> + 1], ..., <i>a</i>[<i>r</i><sub class="lower-index"><i>i</i></sub>]</span>.</p><p>Alyona is going to find <span class="tex-font-style-it">mex</span> for each of the chosen subarrays. Among these <span class="tex-span"><i>m</i></span> <span class="tex-font-style-it">mexes</span> the girl is going to find the smallest. She wants this minimum <span class="tex-font-style-it">mex</span> to be as large as possible. </p><p>You are to find an array <span class="tex-span"><i>a</i></span> of <span class="tex-span"><i>n</i></span> elements so that the minimum <span class="tex-font-style-it">mex</span> among those chosen by Alyona subarrays is as large as possible.</p><p>The <span class="tex-font-style-it">mex</span> of a set <span class="tex-span"><i>S</i></span> is a minimum possible non-negative integer that is not in <span class="tex-span"><i>S</i></span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The next <span class="tex-span"><i>m</i></span> lines contain information about the subarrays chosen by Alyona. The <span class="tex-span"><i>i</i></span>-th of these lines contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), that describe the subarray <span class="tex-span"><i>a</i>[<i>l</i><sub class="lower-index"><i>i</i></sub>], <i>a</i>[<i>l</i><sub class="lower-index"><i>i</i></sub> + 1], ..., <i>a</i>[<i>r</i><sub class="lower-index"><i>i</i></sub>]</span>.</p></div><div class="output-specification"><p>In the first line print single integer&nbsp;— the maximum possible minimum <span class="tex-font-style-it">mex</span>.</p><p>In the second line print <span class="tex-span"><i>n</i></span> integers&nbsp;— the array <span class="tex-span"><i>a</i></span>. All the elements in <span class="tex-span"><i>a</i></span> should be between <span class="tex-span">0</span> and <span class="tex-span">10<sup class="upper-index">9</sup></span>.</p><p>It is guaranteed that there is an optimal answer in which all the elements in <span class="tex-span"><i>a</i></span> are between <span class="tex-span">0</span> and <span class="tex-span">10<sup class="upper-index">9</sup></span>.</p><p>If there are multiple solutions, print any of them.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The next <span class="tex-span"><i>m</i></span> lines contain information about the subarrays chosen by Alyona. The <span class="tex-span"><i>i</i></span>-th of these lines contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), that describe the subarray <span class="tex-span"><i>a</i>[<i>l</i><sub class="lower-index"><i>i</i></sub>], <i>a</i>[<i>l</i><sub class="lower-index"><i>i</i></sub> + 1], ..., <i>a</i>[<i>r</i><sub class="lower-index"><i>i</i></sub>]</span>.</p>

## Output

<p>In the first line print single integer&nbsp;— the maximum possible minimum <span class="tex-font-style-it">mex</span>.</p><p>In the second line print <span class="tex-span"><i>n</i></span> integers&nbsp;— the array <span class="tex-span"><i>a</i></span>. All the elements in <span class="tex-span"><i>a</i></span> should be between <span class="tex-span">0</span> and <span class="tex-span">10<sup class="upper-index">9</sup></span>.</p><p>It is guaranteed that there is an optimal answer in which all the elements in <span class="tex-span"><i>a</i></span> are between <span class="tex-span">0</span> and <span class="tex-span">10<sup class="upper-index">9</sup></span>.</p><p>If there are multiple solutions, print any of them.</p>





```input1
5 3
1 3
2 5
4 5

```




```input2
4 2
1 4
2 4

```




```output1
2
1 0 2 1 0

```




```output2
3
5 2 0 1
```



## Note

<p>The first example: the <span class="tex-font-style-it">mex</span> of the subarray <span class="tex-span">(1, 3)</span> is equal to <span class="tex-span">3</span>, the <span class="tex-font-style-it">mex</span> of the subarray <span class="tex-span">(2, 5)</span> is equal to <span class="tex-span">3</span>, the <span class="tex-font-style-it">mex</span> of the subarray <span class="tex-span">(4, 5)</span> is equal to <span class="tex-span">2</span> as well, thus the minumal <span class="tex-font-style-it">mex</span> among the subarrays chosen by Alyona is equal to <span class="tex-span">2</span>.</p>
