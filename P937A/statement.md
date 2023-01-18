## Description

<div><p>The recent All-Berland Olympiad in Informatics featured <span class="tex-span"><i>n</i></span> participants with each scoring a certain amount of points.</p><p>As the head of the programming committee, you are to determine the set of participants to be awarded with diplomas with respect to the following criteria: </p><ul> <li> At least one participant should get a diploma. </li><li> None of those with score equal to zero should get awarded. </li><li> When someone is awarded, all participants with score <span class="tex-font-style-bf">not less</span> than his score should also be awarded. </li></ul><p>Determine the number of ways to choose a subset of participants that will receive the diplomas.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the number of participants.</p><p>The next line contains a sequence of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 600</span>)&nbsp;— participants' scores.</p><p>It's guaranteed that at least one participant has non-zero score.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the desired number of ways.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the number of participants.</p><p>The next line contains a sequence of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 600</span>)&nbsp;— participants' scores.</p><p>It's guaranteed that at least one participant has non-zero score.</p>

## Output

<p>Print a single integer&nbsp;— the desired number of ways.</p>





```input1
4
1 3 3 2

```




```input2
3
1 1 1

```




```input3
4
42 0 0 42

```




```output1
3

```




```output2
1

```




```output3
1

```



## Note

<p>There are three ways to choose a subset in sample case one.</p><ol> <li> Only participants with 3 points will get diplomas. </li><li> Participants with 2 or 3 points will get diplomas. </li><li> Everyone will get a diploma! </li></ol><p>The only option in sample case two is to award everyone.</p><p>Note that in sample case three participants with zero scores cannot get anything.</p>
