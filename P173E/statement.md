## Description

<div><p>A club wants to take its members camping. In order to organize the event better the club directors decided to partition the members into several groups. </p><p>Club member <span class="tex-span"><i>i</i></span> has a responsibility value <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> and an age value <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. A <span class="tex-font-style-it">group</span> is a non-empty subset of club members with one member known as group leader. A group leader should be one of the most responsible members of the group (his responsibility value is not less than responsibility of any other group member) and his age absolute difference with any other group member should not exceed <span class="tex-span"><i>k</i></span>. </p><p>Some club members are friends and want to be in the same group. They also like their group to be as large as possible. Now you should write a program that answers a series of questions like "What's the largest size of a group containing club member <span class="tex-span"><i>x</i></span> and club member <span class="tex-span"><i>y</i></span>?". It's possible for <span class="tex-span"><i>x</i></span> or <span class="tex-span"><i>y</i></span> to be the group leader.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 0 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>) — the number of club members and the age restriction for one group. </p><p>The next line contains integer numbers <span class="tex-span"><i>r</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">2</sub>, ..., <i>r</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) separated by space: <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> denotes the <span class="tex-span"><i>i</i></span>-th club member's responsibility. In the same way there are integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) in the third line: <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> denotes the <span class="tex-span"><i>i</i></span>-th club member's age.</p><p>The next line contains an integer <span class="tex-span"><i>q</i></span> denoting the number of questions that you should answer (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>). The next <span class="tex-span"><i>q</i></span> lines describe the questions. Each line contains two space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>x</i><sub class="lower-index"><i>i</i></sub> ≠ <i>y</i><sub class="lower-index"><i>i</i></sub></span>) — the indices of the club members that should end up in the same group. </p></div><div class="output-specification"><p>For each question print the maximum size of the group in a line. If making such a group is impossible print -1 instead.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 0 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>) — the number of club members and the age restriction for one group. </p><p>The next line contains integer numbers <span class="tex-span"><i>r</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">2</sub>, ..., <i>r</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) separated by space: <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> denotes the <span class="tex-span"><i>i</i></span>-th club member's responsibility. In the same way there are integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) in the third line: <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> denotes the <span class="tex-span"><i>i</i></span>-th club member's age.</p><p>The next line contains an integer <span class="tex-span"><i>q</i></span> denoting the number of questions that you should answer (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>). The next <span class="tex-span"><i>q</i></span> lines describe the questions. Each line contains two space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>x</i><sub class="lower-index"><i>i</i></sub> ≠ <i>y</i><sub class="lower-index"><i>i</i></sub></span>) — the indices of the club members that should end up in the same group. </p>

## Output

<p>For each question print the maximum size of the group in a line. If making such a group is impossible print -1 instead.</p>





```input1
5 1
1 5 4 1 2
4 4 3 2 2
4
5 3
2 3
2 5
4 1

```




```output1
4
3
-1
4

```



## Note

<p>In the first query the largest group with members 3 and 5 is <span class="tex-span">{1, 3, 4, 5}</span> where member 3 is the leader.</p><p>In the second query member 2 should be the leader so the group will be <span class="tex-span">{1, 2, 3}</span>.</p><p>In the third query the leader of the group should have age 3 so the only leader can be member 3, who is less responsible than member 2. So making a group is impossible.</p><p>The group for the fourth query is the same as first query.</p>
