## Description

<div><p>Little Alyona is celebrating Happy Birthday! Her mother has an array of <span class="tex-span"><i>n</i></span> flowers. Each flower has some mood, the mood of <span class="tex-span"><i>i</i></span>-th flower is <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. The mood can be positive, zero or negative.</p><p>Let's define a subarray as a segment of consecutive flowers. The mother suggested some set of subarrays. Alyona wants to choose several of the subarrays suggested by her mother. After that, each of the flowers will add to the girl's happiness its mood multiplied by the number of chosen subarrays the flower is in.</p><p>For example, consider the case when the mother has <span class="tex-span">5</span> flowers, and their moods are equal to <span class="tex-span">1,  - 2, 1, 3,  - 4</span>. Suppose the mother suggested subarrays <span class="tex-span">(1,  - 2)</span>, <span class="tex-span">(3,  - 4)</span>, <span class="tex-span">(1, 3)</span>, <span class="tex-span">(1,  - 2, 1, 3)</span>. Then if the girl chooses the third and the fourth subarrays then: </p><ul> <li> the first flower adds <span class="tex-span">1·1 = 1</span> to the girl's happiness, because he is in one of chosen subarrays, </li><li> the second flower adds <span class="tex-span">( - 2)·1 =  - 2</span>, because he is in one of chosen subarrays, </li><li> the third flower adds <span class="tex-span">1·2 = 2</span>, because he is in two of chosen subarrays, </li><li> the fourth flower adds <span class="tex-span">3·2 = 6</span>, because he is in two of chosen subarrays, </li><li> the fifth flower adds <span class="tex-span">( - 4)·0 = 0</span>, because he is in no chosen subarrays. </li></ul><p>Thus, in total <span class="tex-span">1 + ( - 2) + 2 + 6 + 0 = 7</span> is added to the girl's happiness. Alyona wants to choose such subarrays from those suggested by the mother that the value added to her happiness would be as large as possible. Help her do this!</p><p>Alyona can choose any number of the subarrays, even <span class="tex-span">0</span> or all suggested by her mother.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>)&nbsp;— the number of flowers and the number of subarrays suggested by the mother.</p><p>The second line contains the flowers moods&nbsp;— <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 100 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>).</p><p>The next <span class="tex-span"><i>m</i></span> lines contain the description of the subarrays suggested by the mother. The <span class="tex-span"><i>i</i></span>-th of these lines contain two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) denoting the subarray <span class="tex-span"><i>a</i>[<i>l</i><sub class="lower-index"><i>i</i></sub>], <i>a</i>[<i>l</i><sub class="lower-index"><i>i</i></sub> + 1], ..., <i>a</i>[<i>r</i><sub class="lower-index"><i>i</i></sub>]</span>.</p><p>Each subarray can encounter more than once.</p></div><div class="output-specification"><p>Print single integer&nbsp;— the maximum possible value added to the Alyona's happiness.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>)&nbsp;— the number of flowers and the number of subarrays suggested by the mother.</p><p>The second line contains the flowers moods&nbsp;— <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 100 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>).</p><p>The next <span class="tex-span"><i>m</i></span> lines contain the description of the subarrays suggested by the mother. The <span class="tex-span"><i>i</i></span>-th of these lines contain two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) denoting the subarray <span class="tex-span"><i>a</i>[<i>l</i><sub class="lower-index"><i>i</i></sub>], <i>a</i>[<i>l</i><sub class="lower-index"><i>i</i></sub> + 1], ..., <i>a</i>[<i>r</i><sub class="lower-index"><i>i</i></sub>]</span>.</p><p>Each subarray can encounter more than once.</p>

## Output

<p>Print single integer&nbsp;— the maximum possible value added to the Alyona's happiness.</p>





```input1
5 4
1 -2 1 3 -4
1 2
4 5
3 4
1 4

```




```input2
4 3
1 2 3 4
1 3
2 4
1 1

```




```input3
2 2
-1 -2
1 1
1 2

```




```output1
7

```




```output2
16

```




```output3
0

```



## Note

<p>The first example is the situation described in the statements.</p><p>In the second example Alyona should choose all subarrays.</p><p>The third example has answer <span class="tex-span">0</span> because Alyona can choose none of the subarrays.</p>
