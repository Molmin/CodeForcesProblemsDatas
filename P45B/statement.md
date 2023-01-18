## Description

<div><p>There are <span class="tex-span"><i>n</i></span> students studying in the 6th grade, in group "B" of a berland secondary school. Every one of them has exactly one friend whom he calls when he has some news. Let us denote the friend of the person number <span class="tex-span"><i>i</i></span> by <span class="tex-span"><i>g</i>(<i>i</i>)</span>. Note that the friendships are not mutual, i.e. <span class="tex-span"><i>g</i>(<i>g</i>(<i>i</i>))</span> is not necessarily equal to <span class="tex-span"><i>i</i></span>.</p><p>On day <span class="tex-span"><i>i</i></span> the person numbered as <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> learns the news with the rating of <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub> ≥ 1</span>). He phones the friend immediately and tells it. While he is doing it, the news becomes old and its rating falls a little and becomes equal to <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub> - 1</span>. The friend does the same thing — he also calls his friend and also tells the news. The friend of the friend gets the news already rated as <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub> - 2</span>. It all continues until the rating of the news reaches zero as nobody wants to tell the news with zero rating. </p><p>More formally, everybody acts like this: if a person <span class="tex-span"><i>x</i></span> learns the news with a non-zero rating <span class="tex-span"><i>y</i></span>, he calls his friend <span class="tex-span"><i>g</i>(<i>i</i>)</span> and his friend learns the news with the rating of <span class="tex-span"><i>y</i> - 1</span> and, if it is possible, continues the process.</p><p>Let us note that during a day one and the same person may call his friend and tell him one and the same news with different ratings. Thus, the news with the rating of <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> will lead to as much as <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> calls.</p><p>Your task is to count the values of <span class="tex-span"><i>res</i><sub class="lower-index"><i>i</i></sub></span> — how many students learned their first news on day <span class="tex-span"><i>i</i></span>.</p><p>The values of <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> are known initially, whereas <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is determined from the following formula: </p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://zLM4hbTw.png" style="max-width: 100.0%;max-height: 100.0%;"></center> where mod stands for the operation of taking the excess from the cleavage, <span class="tex-span"><i>res</i><sub class="lower-index">0</sub></span> is considered equal to zero and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> — some given integers.</div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of students and the number of days. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>g</i>(<i>i</i>)</span> (<span class="tex-span">1 ≤ <i>g</i>(<i>i</i>) ≤ <i>n</i>, <i>g</i>(<i>i</i>) ≠ <i>i</i></span>) — the number of a friend of the <span class="tex-span"><i>i</i></span>-th student. The third line contains <span class="tex-span"><i>m</i></span> space-separated integers <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">7</sup></span>). The fourth line contains <span class="tex-span"><i>m</i></span> space-separated integers <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">7</sup></span>).</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> lines containing one number each. The <span class="tex-span"><i>i</i></span>-th line should contain <span class="tex-span"><i>res</i><sub class="lower-index"><i>i</i></sub></span> — for what number of students the first news they've learned over the <span class="tex-span"><i>m</i></span> days in question, was the news number <span class="tex-span"><i>i</i></span>. The number of the news is the number of the day on which it can be learned. The days are numbered starting from one in the order in which they are given in the input file. Don't output <span class="tex-span"><i>res</i><sub class="lower-index">0</sub></span>.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of students and the number of days. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>g</i>(<i>i</i>)</span> (<span class="tex-span">1 ≤ <i>g</i>(<i>i</i>) ≤ <i>n</i>, <i>g</i>(<i>i</i>) ≠ <i>i</i></span>) — the number of a friend of the <span class="tex-span"><i>i</i></span>-th student. The third line contains <span class="tex-span"><i>m</i></span> space-separated integers <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">7</sup></span>). The fourth line contains <span class="tex-span"><i>m</i></span> space-separated integers <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">7</sup></span>).</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> lines containing one number each. The <span class="tex-span"><i>i</i></span>-th line should contain <span class="tex-span"><i>res</i><sub class="lower-index"><i>i</i></sub></span> — for what number of students the first news they've learned over the <span class="tex-span"><i>m</i></span> days in question, was the news number <span class="tex-span"><i>i</i></span>. The number of the news is the number of the day on which it can be learned. The days are numbered starting from one in the order in which they are given in the input file. Don't output <span class="tex-span"><i>res</i><sub class="lower-index">0</sub></span>.</p>





```input1
3 4
2 3 1
1 2 3 4
1 2 3 4

```




```input2
8 6
7 6 4 2 3 5 5 7
10 4 3 8 9 1
1 1 1 2 2 2

```




```output1
1
1
1
0

```




```output2
1
1
1
2
1
1

```


