## Description

<div><p>In a kindergarten, the children are being divided into groups. The teacher put the children in a line and associated each child with his or her integer charisma value. Each child should go to exactly one group. Each group should be a nonempty segment of consecutive children of a line. A group's <span class="tex-font-style-underline">sociability</span> is the maximum difference of charisma of two children in the group (in particular, if the group consists of one child, its sociability equals a zero). </p><p>The teacher wants to divide the children into some number of groups in such way that the total <span class="tex-font-style-underline">sociability</span> of the groups is maximum. Help him find this value.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span>&nbsp;— the number of children in the line (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— the charisma of the <span class="tex-span"><i>i</i></span>-th child (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Print the maximum possible total sociability of all groups.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span>&nbsp;— the number of children in the line (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— the charisma of the <span class="tex-span"><i>i</i></span>-th child (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Print the maximum possible total sociability of all groups.</p>





```input1
5
1 2 3 1 2

```




```input2
3
3 3 3

```




```output1
3

```




```output2
0

```



## Note

<p>In the first test sample one of the possible variants of an division is following: the first three children form a group with sociability 2, and the two remaining children form a group with sociability 1.</p><p>In the second test sample any division leads to the same result, the sociability will be equal to 0 in each group.</p>
