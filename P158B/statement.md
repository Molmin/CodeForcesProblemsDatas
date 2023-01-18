## Description

<div><p>After the lessons <span class="tex-span"><i>n</i></span> groups of schoolchildren went outside and decided to visit Polycarpus to celebrate his birthday. We know that the <span class="tex-span"><i>i</i></span>-th group consists of <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> friends (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 4</span>), and they want to go to Polycarpus together. They decided to get there by taxi. Each car can carry at most four passengers. What minimum number of cars will the children need if all members of each group should ride in the same taxi (but one taxi can take more than one group)?</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of groups of schoolchildren. The second line contains a sequence of integers <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 4</span>). The integers are separated by a space, <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> is the number of children in the <span class="tex-span"><i>i</i></span>-th group.</p></div><div class="output-specification"><p>Print the single number — the minimum number of taxis necessary to drive all children to Polycarpus.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of groups of schoolchildren. The second line contains a sequence of integers <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 4</span>). The integers are separated by a space, <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> is the number of children in the <span class="tex-span"><i>i</i></span>-th group.</p>

## Output

<p>Print the single number — the minimum number of taxis necessary to drive all children to Polycarpus.</p>





```input1
5
1 2 4 3 3

```




```input2
8
2 3 4 4 2 1 3 1

```




```output1
4

```




```output2
5

```



## Note

<p>In the first test we can sort the children into four cars like this:</p><ul> <li> the third group (consisting of four children), </li><li> the fourth group (consisting of three children), </li><li> the fifth group (consisting of three children), </li><li> the first and the second group (consisting of one and two children, correspondingly). </li></ul><p>There are other ways to sort the groups into four cars.</p>
