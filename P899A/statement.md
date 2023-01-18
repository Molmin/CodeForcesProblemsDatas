## Description

<div><p>There were <span class="tex-span"><i>n</i></span> groups of students which came to write a training contest. A group is either one person who can write the contest with anyone else, or two people who want to write the contest in the same team.</p><p>The coach decided to form teams of exactly three people for this training. Determine the maximum number of teams of three people he can form. It is possible that he can't use all groups to form teams. For groups of two, either both students should write the contest, or both should not. If two students from a group of two will write the contest, they should be in the same team.</p></div><div class="input-specification"><p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of groups.</p><p>The second line contains a sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 2</span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number of people in group <span class="tex-span"><i>i</i></span>.</p></div><div class="output-specification"><p>Print the maximum number of teams of three people the coach can form.</p></div>

## Input

<p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of groups.</p><p>The second line contains a sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 2</span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number of people in group <span class="tex-span"><i>i</i></span>.</p>

## Output

<p>Print the maximum number of teams of three people the coach can form.</p>





```input1
4
1 1 2 1

```




```input2
2
2 2

```




```input3
7
2 2 2 1 1 1 1

```




```input4
3
1 1 1

```




```output1
1

```




```output2
0

```




```output3
3

```




```output4
1

```



## Note

<p>In the first example the coach can form one team. For example, he can take students from the first, second and fourth groups.</p><p>In the second example he can't make a single team.</p><p>In the third example the coach can form three teams. For example, he can do this in the following way:</p><ul> <li> The first group (of two people) and the seventh group (of one person), </li><li> The second group (of two people) and the sixth group (of one person), </li><li> The third group (of two people) and the fourth group (of one person). </li></ul>
