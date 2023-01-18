## Description

<div><p>Drazil and Varda are the earthworm couple. They want to find a good place to bring up their children. They found a good ground containing nature hole. The hole contains many rooms, some pairs of rooms are connected by small tunnels such that earthworm can move between them.</p><p>Let's consider rooms and small tunnels as the vertices and edges in a graph. This graph is a <span class="tex-font-style-underline">tree</span>. In the other words, any pair of vertices has an unique path between them.</p><p>Each room that is <span class="tex-font-style-underline">leaf</span> in the graph is connected with a ground by a vertical tunnel. Here, <span class="tex-font-style-underline">leaf</span> is a vertex that has only one outgoing edge in the graph.</p><p>Each room is large enough only to fit one earthworm living in it. Earthworm can't live in a tunnel.</p><p>Drazil and Varda have a plan to educate their children. They want all their children to do morning exercises immediately after getting up!</p><p>When the morning is coming, all earthworm children get up in the same time, then each of them chooses the <span class="tex-font-style-bf">farthest</span> path to the ground for gathering with others (these children are lazy, so they all want to do exercises as late as possible).</p><p>Drazil and Varda want the difference between the time first earthworm child arrives outside and the time the last earthworm child arrives outside to be not larger than <span class="tex-span"><i>l</i></span> (otherwise children will spread around the ground and it will be hard to keep them exercising together).</p><p>Also, The rooms that are occupied by their children should form a <span class="tex-font-style-underline">connected</span> set. In the other words, for any two rooms that are occupied with earthworm children, all rooms that lie on the path between them should be occupied with earthworm children too.</p><p>How many children Drazil and Varda may have at most in order to satisfy all conditions above? Drazil and Varda want to know the answer for many different choices of <span class="tex-span"><i>l</i></span>.</p><p>(Drazil and Varda don't live in the hole with their children)</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>n</i></span> denoting how many rooms there are in the hole (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>Then there are <span class="tex-span"><i>n</i> - 1</span> lines following. Each of these lines contains three integers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span>, <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>v</i> ≤ 10<sup class="upper-index">6</sup></span>) denoting there is a small tunnel between room <span class="tex-span"><i>x</i></span> and room <span class="tex-span"><i>y</i></span> that takes time <span class="tex-span"><i>v</i></span> to pass. </p><p>Suppose that the time for an earthworm to get out to the ground from any leaf room is the same.</p><p>The next line contains an integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 50</span>), denoting the number of different value of <span class="tex-span"><i>l</i></span> you need to process.</p><p>The last line contains <span class="tex-span"><i>q</i></span> numbers, each number denoting a value of <span class="tex-span"><i>l</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ 10<sup class="upper-index">11</sup></span>).</p></div><div class="output-specification"><p>You should print <span class="tex-span"><i>q</i></span> lines. Each line should contain one integer denoting the answer for a corresponding value of <span class="tex-span"><i>l</i></span>.</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>n</i></span> denoting how many rooms there are in the hole (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>Then there are <span class="tex-span"><i>n</i> - 1</span> lines following. Each of these lines contains three integers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span>, <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>v</i> ≤ 10<sup class="upper-index">6</sup></span>) denoting there is a small tunnel between room <span class="tex-span"><i>x</i></span> and room <span class="tex-span"><i>y</i></span> that takes time <span class="tex-span"><i>v</i></span> to pass. </p><p>Suppose that the time for an earthworm to get out to the ground from any leaf room is the same.</p><p>The next line contains an integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 50</span>), denoting the number of different value of <span class="tex-span"><i>l</i></span> you need to process.</p><p>The last line contains <span class="tex-span"><i>q</i></span> numbers, each number denoting a value of <span class="tex-span"><i>l</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ 10<sup class="upper-index">11</sup></span>).</p>

## Output

<p>You should print <span class="tex-span"><i>q</i></span> lines. Each line should contain one integer denoting the answer for a corresponding value of <span class="tex-span"><i>l</i></span>.</p>





```input1
5
1 2 3
2 3 4
4 5 3
3 4 2
5
1 2 3 4 5

```




```input2
12
5 9 3
2 1 7
11 7 2
6 5 5
2 5 3
6 7 2
1 4 4
8 5 7
1 3 8
11 12 3
10 8 2
10
13 14 14 13 13 4 6 7 2 1

```




```output1
1
3
3
3
5

```




```output2
10
10
10
10
10
3
3
5
2
1

```



## Note

<p>For the first sample the hole looks like the following. Rooms 1 and 5 are leaves, so they contain a vertical tunnel connecting them to the ground. The lengths of farthest path from rooms <span class="tex-span">1 – 5</span> to the ground are <span class="tex-span">12, 9, 7, 9, 12</span> respectively. </p><p>If l = 1, we may only choose any single room. </p><p>If l = 2..4, we may choose rooms 2, 3, and 4 as the answer. </p><p>If l = 5, we may choose all rooms.</p><center><img class="tex-graphics" src="file://inQ7x8CK.png" style="max-width: 100.0%;max-height: 100.0%;"></center>
