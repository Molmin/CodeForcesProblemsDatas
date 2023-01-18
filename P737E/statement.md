## Description

<div><p>Tanya is now five so all her friends gathered together to celebrate her birthday. There are <span class="tex-span"><i>n</i></span> children on the celebration, including Tanya.</p><p>The celebration is close to its end, and the last planned attraction is gaming machines. There are <span class="tex-span"><i>m</i></span> machines in the hall, they are numbered <span class="tex-span">1</span> through <span class="tex-span"><i>m</i></span>. Each of the children has a list of machines he wants to play on. Moreover, for each of the machines he knows the exact time he wants to play on it. For every machine, no more than one child can play on this machine at the same time.</p><p>It is evening already, so every adult wants to go home. To speed up the process, you can additionally rent second copies of each of the machines. To rent the second copy of the <span class="tex-span"><i>j</i></span>-th machine, you have to pay <span class="tex-span"><i>p</i><sub class="lower-index"><i>j</i></sub></span> burles. After you rent a machine, you can use it for as long as you want.</p><p>How long it will take to make every child play according to his plan, if you have a budget of <span class="tex-span"><i>b</i></span> burles for renting additional machines? There is only one copy of each machine, so it's impossible to rent a third machine of the same type.</p><p>The children can interrupt the game in any moment and continue it later. If the <span class="tex-span"><i>i</i></span>-th child wants to play on the <span class="tex-span"><i>j</i></span>-th machine, it is allowed after you rent the copy of the <span class="tex-span"><i>j</i></span>-th machine that this child would play some part of the time on the <span class="tex-span"><i>j</i></span>-th machine and some part of the time on its copy (each of these parts could be empty). The interruptions and changes take no time and can be performed in any integer moment of time. Of course, a child can't play on more than one machine at the same time.</p><p>Remember, that it is not needed to save money (no one saves money at the expense of children happiness!), it is needed to minimize the latest moment of time some child ends his game.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 40</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 10</span>, <span class="tex-span">0 ≤ <i>b</i> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;— the number of children, the number of gaming machines and the budget for renting additional machines.</p><p>The second line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">6</sup></span>), where <span class="tex-span"><i>p</i><sub class="lower-index"><i>j</i></sub></span> is the rent price for the second copy of the <span class="tex-span"><i>j</i></span>-th machine.</p><p><span class="tex-span"><i>n</i></span> lines follow, <span class="tex-span"><i>i</i></span>-th of them describes the wishes of the <span class="tex-span"><i>i</i></span>-th child. The line starts with an integer <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>)&nbsp;— the number of machines, the <span class="tex-span"><i>i</i></span>-th child wants to play on. Then there are <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> pairs in the line, the <span class="tex-span"><i>y</i></span>-th of them is <span class="tex-span"><i>x</i><sub class="lower-index"><i>iy</i></sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index"><i>iy</i></sub></span>. It means that, the <span class="tex-span"><i>i</i></span>-th child wants to play <span class="tex-span"><i>t</i><sub class="lower-index"><i>iy</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>iy</i></sub> ≤ 2500</span>) minutes on the <span class="tex-span"><i>x</i><sub class="lower-index"><i>iy</i></sub></span>-th (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>iy</i></sub> ≤ <i>m</i></span>) machine. In each of these <span class="tex-span"><i>n</i></span> lines the values <span class="tex-span"><i>x</i><sub class="lower-index"><i>iy</i></sub></span> are distinct.</p></div><div class="output-specification"><p>In the first line print the minimum time in which all the children can finish their games.</p><p>In the second line print a string of length <span class="tex-span"><i>m</i></span> consisting of zeros and ones. The <span class="tex-span"><i>j</i></span>-th character is '<span class="tex-font-style-tt">1</span>', if the copy of <span class="tex-span"><i>j</i></span>-th machine should be rated, and '<span class="tex-font-style-tt">0</span>' otherwise.</p><p>In the third line print integer <span class="tex-span"><i>g</i></span> (<span class="tex-span">0 ≤ <i>g</i> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;— the total number of time segments of continuous playing for all of the children. Then in <span class="tex-span"><i>g</i></span> lines print the segments as four integers <span class="tex-span"><i>i</i></span>, <span class="tex-span"><i>j</i></span>, <span class="tex-span"><i>s</i></span>, <span class="tex-span"><i>d</i></span>, meaning that the <span class="tex-span"><i>i</i></span>-th child was playing on the <span class="tex-span"><i>j</i></span>-th machine or its copy from the time moment <span class="tex-span"><i>s</i></span> (<span class="tex-span"><i>s</i> ≥ 0</span>) for <span class="tex-span"><i>d</i></span> minutes (<span class="tex-span"><i>d</i> ≥ 1</span>). You can print these lines in arbitrary order.</p><p>If there are multiple answers, print any of them.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 40</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 10</span>, <span class="tex-span">0 ≤ <i>b</i> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;— the number of children, the number of gaming machines and the budget for renting additional machines.</p><p>The second line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">6</sup></span>), where <span class="tex-span"><i>p</i><sub class="lower-index"><i>j</i></sub></span> is the rent price for the second copy of the <span class="tex-span"><i>j</i></span>-th machine.</p><p><span class="tex-span"><i>n</i></span> lines follow, <span class="tex-span"><i>i</i></span>-th of them describes the wishes of the <span class="tex-span"><i>i</i></span>-th child. The line starts with an integer <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>)&nbsp;— the number of machines, the <span class="tex-span"><i>i</i></span>-th child wants to play on. Then there are <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> pairs in the line, the <span class="tex-span"><i>y</i></span>-th of them is <span class="tex-span"><i>x</i><sub class="lower-index"><i>iy</i></sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index"><i>iy</i></sub></span>. It means that, the <span class="tex-span"><i>i</i></span>-th child wants to play <span class="tex-span"><i>t</i><sub class="lower-index"><i>iy</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>iy</i></sub> ≤ 2500</span>) minutes on the <span class="tex-span"><i>x</i><sub class="lower-index"><i>iy</i></sub></span>-th (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>iy</i></sub> ≤ <i>m</i></span>) machine. In each of these <span class="tex-span"><i>n</i></span> lines the values <span class="tex-span"><i>x</i><sub class="lower-index"><i>iy</i></sub></span> are distinct.</p>

## Output

<p>In the first line print the minimum time in which all the children can finish their games.</p><p>In the second line print a string of length <span class="tex-span"><i>m</i></span> consisting of zeros and ones. The <span class="tex-span"><i>j</i></span>-th character is '<span class="tex-font-style-tt">1</span>', if the copy of <span class="tex-span"><i>j</i></span>-th machine should be rated, and '<span class="tex-font-style-tt">0</span>' otherwise.</p><p>In the third line print integer <span class="tex-span"><i>g</i></span> (<span class="tex-span">0 ≤ <i>g</i> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;— the total number of time segments of continuous playing for all of the children. Then in <span class="tex-span"><i>g</i></span> lines print the segments as four integers <span class="tex-span"><i>i</i></span>, <span class="tex-span"><i>j</i></span>, <span class="tex-span"><i>s</i></span>, <span class="tex-span"><i>d</i></span>, meaning that the <span class="tex-span"><i>i</i></span>-th child was playing on the <span class="tex-span"><i>j</i></span>-th machine or its copy from the time moment <span class="tex-span"><i>s</i></span> (<span class="tex-span"><i>s</i> ≥ 0</span>) for <span class="tex-span"><i>d</i></span> minutes (<span class="tex-span"><i>d</i> ≥ 1</span>). You can print these lines in arbitrary order.</p><p>If there are multiple answers, print any of them.</p>





```input1
2 2 100
3 7
2 1 3 2 1
2 1 3 2 1

```




```input2
3 2 15
11 7
2 2 10 1 5
1 2 20
2 1 4 2 3

```




```output1
4
10
8
1 1 0 1
2 2 0 1
1 1 1 1
2 1 1 1
2 1 2 1
1 1 2 1
1 2 3 1
2 1 3 1

```




```output2
20
01
17
2 2 0 4
2 2 4 1
1 1 5 2
2 2 5 2
1 2 7 5
2 2 7 5
2 2 12 1
1 2 12 1
3 1 13 4
2 2 13 4
1 2 13 4
1 1 17 2
3 2 17 2
2 2 17 2
1 1 19 1
2 2 19 1
3 2 19 1

```


