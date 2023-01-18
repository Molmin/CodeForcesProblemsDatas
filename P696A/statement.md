## Description

<div><p>Barney lives in NYC. NYC has infinite number of intersections numbered with positive integers starting from 1. There exists a bidirectional road between intersections <span class="tex-span"><i>i</i></span> and <span class="tex-span">2<i>i</i></span> and another road between <span class="tex-span"><i>i</i></span> and <span class="tex-span">2<i>i</i> + 1</span> for every positive integer <span class="tex-span"><i>i</i></span>. You can clearly see that there exists a unique shortest path between any two intersections.</p><center> <img class="tex-graphics" src="file://V1vO1tyu.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Initially anyone can pass any road for free. But since SlapsGiving is ahead of us, there will <span class="tex-span"><i>q</i></span> consecutive events happen soon. There are two types of events:</p><p>1. Government makes a new rule. A rule can be denoted by integers <span class="tex-span"><i>v</i></span>, <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>w</i></span>. As the result of this action, the passing fee of all roads on the shortest path from <span class="tex-span"><i>u</i></span> to <span class="tex-span"><i>v</i></span> increases by <span class="tex-span"><i>w</i></span> dollars. </p><p>2. Barney starts moving from some intersection <span class="tex-span"><i>v</i></span> and goes to intersection <span class="tex-span"><i>u</i></span> where there's a girl he wants to cuddle (using his fake name Lorenzo Von Matterhorn). He always uses the shortest path (visiting minimum number of intersections or roads) between two intersections.</p><p>Government needs your calculations. For each time Barney goes to cuddle a girl, you need to tell the government how much money he should pay (sum of passing fee of all roads he passes).</p></div><div class="input-specification"><p>The first line of input contains a single integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 1 000</span>).</p><p>The next <span class="tex-span"><i>q</i></span> lines contain the information about the events in chronological order. Each event is described in form <span class="tex-span">1</span> <span class="tex-span"><i>v</i></span> <span class="tex-span"><i>u</i></span> <span class="tex-span"><i>w</i></span> if it's an event when government makes a new rule about increasing the passing fee of all roads on the shortest path from <span class="tex-span"><i>u</i></span> to <span class="tex-span"><i>v</i></span> by <span class="tex-span"><i>w</i></span> dollars, or in form <span class="tex-span">2</span> <span class="tex-span"><i>v</i></span> <span class="tex-span"><i>u</i></span> if it's an event when Barnie goes to cuddle from the intersection <span class="tex-span"><i>v</i></span> to the intersection <span class="tex-span"><i>u</i></span>.</p><p><span class="tex-span">1 ≤ <i>v</i>, <i>u</i> ≤ 10<sup class="upper-index">18</sup>, <i>v</i> ≠ <i>u</i>, 1 ≤ <i>w</i> ≤ 10<sup class="upper-index">9</sup></span> states for every description line.</p></div><div class="output-specification"><p>For each event of second type print the sum of passing fee of all roads Barney passes in this event, in one line. Print the answers in chronological order of corresponding events.</p></div>

## Input

<p>The first line of input contains a single integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 1 000</span>).</p><p>The next <span class="tex-span"><i>q</i></span> lines contain the information about the events in chronological order. Each event is described in form <span class="tex-span">1</span> <span class="tex-span"><i>v</i></span> <span class="tex-span"><i>u</i></span> <span class="tex-span"><i>w</i></span> if it's an event when government makes a new rule about increasing the passing fee of all roads on the shortest path from <span class="tex-span"><i>u</i></span> to <span class="tex-span"><i>v</i></span> by <span class="tex-span"><i>w</i></span> dollars, or in form <span class="tex-span">2</span> <span class="tex-span"><i>v</i></span> <span class="tex-span"><i>u</i></span> if it's an event when Barnie goes to cuddle from the intersection <span class="tex-span"><i>v</i></span> to the intersection <span class="tex-span"><i>u</i></span>.</p><p><span class="tex-span">1 ≤ <i>v</i>, <i>u</i> ≤ 10<sup class="upper-index">18</sup>, <i>v</i> ≠ <i>u</i>, 1 ≤ <i>w</i> ≤ 10<sup class="upper-index">9</sup></span> states for every description line.</p>

## Output

<p>For each event of second type print the sum of passing fee of all roads Barney passes in this event, in one line. Print the answers in chronological order of corresponding events.</p>





```input1
7
1 3 4 30
1 4 1 2
1 3 6 8
2 4 3
1 6 1 40
2 3 7
2 2 4

```




```output1
94
0
32

```



## Note

<p>In the example testcase:</p><p>Here are the intersections used:</p><center> <img class="tex-graphics" src="file://lduTVY3z.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><ol> <li> Intersections on the path are <span class="tex-span">3</span>, <span class="tex-span">1</span>, <span class="tex-span">2</span> and <span class="tex-span">4</span>. </li><li> Intersections on the path are <span class="tex-span">4</span>, <span class="tex-span">2</span> and <span class="tex-span">1</span>. </li><li> Intersections on the path are only <span class="tex-span">3</span> and <span class="tex-span">6</span>. </li><li> Intersections on the path are <span class="tex-span">4</span>, <span class="tex-span">2</span>, <span class="tex-span">1</span> and <span class="tex-span">3</span>. Passing fee of roads on the path are <span class="tex-span">32</span>, <span class="tex-span">32</span> and <span class="tex-span">30</span> in order. So answer equals to <span class="tex-span">32 + 32 + 30 = 94</span>. </li><li> Intersections on the path are <span class="tex-span">6</span>, <span class="tex-span">3</span> and <span class="tex-span">1</span>. </li><li> Intersections on the path are <span class="tex-span">3</span> and <span class="tex-span">7</span>. Passing fee of the road between them is <span class="tex-span">0</span>. </li><li> Intersections on the path are <span class="tex-span">2</span> and <span class="tex-span">4</span>. Passing fee of the road between them is <span class="tex-span">32</span> (increased by <span class="tex-span">30</span> in the first event and by <span class="tex-span">2</span> in the second). </li></ol>
