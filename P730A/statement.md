## Description

<div><p>A group of <span class="tex-span"><i>n</i></span> friends enjoys playing popular video game Toda 2. There is a rating system describing skill level of each player, initially the rating of the <span class="tex-span"><i>i</i></span>-th friend is <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>The friends decided to take part in the championship as a team. But they should have equal ratings to be allowed to compose a single team consisting of all <span class="tex-span"><i>n</i></span> friends. So the friends are faced with the problem: how to make all their ratings equal.</p><p>One way to change ratings is to willingly lose in some matches. Friends can form a party consisting of <span class="tex-font-style-bf">two</span> to <span class="tex-font-style-bf">five</span> (but not more than <span class="tex-span"><i>n</i></span>) friends and play a match in the game. When the party loses, the rating of each of its members decreases by <span class="tex-span">1</span>. A rating can't become negative, so <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub> = 0</span> doesn't change after losing.</p><p>The friends can take part in multiple matches, each time making a party from any subset of friends (but remember about constraints on party size: from <span class="tex-span">2</span> to <span class="tex-span">5</span> members).</p><p>The friends want to make their ratings equal but as high as possible.</p><p>Help the friends develop a strategy of losing the matches so that all their ratings become equal and the resulting rating is maximum possible.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>) — the number of friends.</p><p>The second line contains <span class="tex-span"><i>n</i></span> non-negative integers <span class="tex-span"><i>r</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">2</sub>, ..., <i>r</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>), where <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> is the initial rating of the <span class="tex-span"><i>i</i></span>-th friend.</p></div><div class="output-specification"><p>In the first line, print a single integer <span class="tex-span"><i>R</i></span> — the final rating of each of the friends.</p><p>In the second line, print integer <span class="tex-span"><i>t</i></span> — the number of matches the friends have to play. Each of the following <span class="tex-span"><i>t</i></span> lines should contain <span class="tex-span"><i>n</i></span> characters '<span class="tex-font-style-tt">0</span>' or '<span class="tex-font-style-tt">1</span>', where the <span class="tex-span"><i>j</i></span>-th character of the <span class="tex-span"><i>i</i></span>-th line is equal to:</p><ul> <li> '<span class="tex-font-style-tt">0</span>', if friend <span class="tex-span"><i>j</i></span> should not play in match <span class="tex-span"><i>i</i></span>, </li><li> '<span class="tex-font-style-tt">1</span>', if friend <span class="tex-span"><i>j</i></span> should play in match <span class="tex-span"><i>i</i></span>. </li></ul><p>Each line should contain between two and five characters '<span class="tex-font-style-tt">1</span>', inclusive.</p><p>The value <span class="tex-span"><i>t</i></span> should not exceed <span class="tex-span">10<sup class="upper-index">4</sup></span>, it is guaranteed that such solution exists. </p><p>Remember that you shouldn't minimize the value <span class="tex-span"><i>t</i></span>, but you should maximize <span class="tex-span"><i>R</i></span>. If there are multiple solutions, print any of them.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>) — the number of friends.</p><p>The second line contains <span class="tex-span"><i>n</i></span> non-negative integers <span class="tex-span"><i>r</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">2</sub>, ..., <i>r</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>), where <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> is the initial rating of the <span class="tex-span"><i>i</i></span>-th friend.</p>

## Output

<p>In the first line, print a single integer <span class="tex-span"><i>R</i></span> — the final rating of each of the friends.</p><p>In the second line, print integer <span class="tex-span"><i>t</i></span> — the number of matches the friends have to play. Each of the following <span class="tex-span"><i>t</i></span> lines should contain <span class="tex-span"><i>n</i></span> characters '<span class="tex-font-style-tt">0</span>' or '<span class="tex-font-style-tt">1</span>', where the <span class="tex-span"><i>j</i></span>-th character of the <span class="tex-span"><i>i</i></span>-th line is equal to:</p><ul> <li> '<span class="tex-font-style-tt">0</span>', if friend <span class="tex-span"><i>j</i></span> should not play in match <span class="tex-span"><i>i</i></span>, </li><li> '<span class="tex-font-style-tt">1</span>', if friend <span class="tex-span"><i>j</i></span> should play in match <span class="tex-span"><i>i</i></span>. </li></ul><p>Each line should contain between two and five characters '<span class="tex-font-style-tt">1</span>', inclusive.</p><p>The value <span class="tex-span"><i>t</i></span> should not exceed <span class="tex-span">10<sup class="upper-index">4</sup></span>, it is guaranteed that such solution exists. </p><p>Remember that you shouldn't minimize the value <span class="tex-span"><i>t</i></span>, but you should maximize <span class="tex-span"><i>R</i></span>. If there are multiple solutions, print any of them.</p>





```input1
5
4 5 1 7 4

```




```input2
2
1 2

```




```input3
3
1 1 1

```




```output1
1
8
01010
00011
01010
10010
00011
11000
00011
11000

```




```output2
0
2
11
11

```




```output3
1
0

```


