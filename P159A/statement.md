## Description

<div><p>Polycarpus has a hobby — he develops an unusual social network. His work is almost completed, and there is only one more module to implement — the module which determines friends. Oh yes, in this social network one won't have to add friends manually! Pairs of friends are deduced in the following way. Let's assume that user <span class="tex-span"><i>A</i></span> sent user <span class="tex-span"><i>B</i></span> a message at time <span class="tex-span"><i>t</i><sub class="lower-index">1</sub></span>, and user <span class="tex-span"><i>B</i></span> sent user <span class="tex-span"><i>A</i></span> a message at time <span class="tex-span"><i>t</i><sub class="lower-index">2</sub></span>. If <span class="tex-span">0 &lt; <i>t</i><sub class="lower-index">2</sub> - <i>t</i><sub class="lower-index">1</sub> ≤ <i>d</i></span>, then user <span class="tex-span"><i>B</i></span>'s message was <span class="tex-font-style-it">an answer</span> to user <span class="tex-span"><i>A</i></span>'s one. Users <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span> are considered to be friends if <span class="tex-span"><i>A</i></span> answered at least one <span class="tex-span"><i>B</i></span>'s message or <span class="tex-span"><i>B</i></span> answered at least one <span class="tex-span"><i>A</i></span>'s message.</p><p>You are given the log of messages in chronological order and a number <span class="tex-span"><i>d</i></span>. Find all pairs of users who will be considered to be friends.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>d</i> ≤ 1000</span>). The next <span class="tex-span"><i>n</i></span> lines contain the messages log. The <span class="tex-span"><i>i</i></span>-th line contains one line of the log formatted as "<span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>B</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>" (without the quotes), which means that user <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i></sub></span> sent a message to user <span class="tex-span"><i>B</i><sub class="lower-index"><i>i</i></sub></span> at time <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>). <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>B</i><sub class="lower-index"><i>i</i></sub></span> are non-empty strings at most <span class="tex-span">20</span> characters long, consisting of lowercase letters ('<span class="tex-font-style-tt">a</span>' ... '<span class="tex-font-style-tt">z</span>'), and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> is an integer (<span class="tex-span">0 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10000</span>). It is guaranteed that the lines are given in non-decreasing order of <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>'s and that no user sent a message to himself. The elements in the lines are separated by single spaces.</p></div><div class="output-specification"><p>In the first line print integer <span class="tex-span"><i>k</i></span> — the number of pairs of friends. In the next <span class="tex-span"><i>k</i></span> lines print pairs of friends as "<span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>B</i><sub class="lower-index"><i>i</i></sub></span>" (without the quotes). You can print users in pairs and the pairs themselves in any order. Each pair must be printed exactly once.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>d</i> ≤ 1000</span>). The next <span class="tex-span"><i>n</i></span> lines contain the messages log. The <span class="tex-span"><i>i</i></span>-th line contains one line of the log formatted as "<span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>B</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>" (without the quotes), which means that user <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i></sub></span> sent a message to user <span class="tex-span"><i>B</i><sub class="lower-index"><i>i</i></sub></span> at time <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>). <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>B</i><sub class="lower-index"><i>i</i></sub></span> are non-empty strings at most <span class="tex-span">20</span> characters long, consisting of lowercase letters ('<span class="tex-font-style-tt">a</span>' ... '<span class="tex-font-style-tt">z</span>'), and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> is an integer (<span class="tex-span">0 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10000</span>). It is guaranteed that the lines are given in non-decreasing order of <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>'s and that no user sent a message to himself. The elements in the lines are separated by single spaces.</p>

## Output

<p>In the first line print integer <span class="tex-span"><i>k</i></span> — the number of pairs of friends. In the next <span class="tex-span"><i>k</i></span> lines print pairs of friends as "<span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>B</i><sub class="lower-index"><i>i</i></sub></span>" (without the quotes). You can print users in pairs and the pairs themselves in any order. Each pair must be printed exactly once.</p>





```input1
4 1
vasya petya 1
petya vasya 2
anya ivan 2
ivan anya 4

```




```input2
1 1000
a b 0

```




```output1
1
petya vasya

```




```output2
0

```



## Note

<p>In the first sample test case Vasya and Petya are friends because their messages' sending times are one second apart. Anya and Ivan are not, because their messages' sending times differ by more than one second.</p>
