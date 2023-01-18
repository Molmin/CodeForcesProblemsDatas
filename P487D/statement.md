## Description

<div><p>Automatic Bakery of Cyberland (ABC) recently bought an <span class="tex-span"><i>n</i> × <i>m</i></span> rectangle table. To serve the diners, ABC placed seats around the table. The size of each seat is equal to a unit square, so there are <span class="tex-span">2(<i>n</i> + <i>m</i>)</span> seats in total.</p><p>ABC placed conveyor belts on each unit square on the table. There are three types of conveyor belts: "<span class="tex-font-style-tt">^</span>", "<span class="tex-font-style-tt">&lt;</span>" and "<span class="tex-font-style-tt">&gt;</span>". A "<span class="tex-font-style-tt">^</span>" belt can bring things upwards. "<span class="tex-font-style-tt">&lt;</span>" can bring leftwards and "<span class="tex-font-style-tt">&gt;</span>" can bring rightwards.</p><p>Let's number the rows with <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from top to bottom, the columns with <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span> from left to right. We consider the seats above and below the top of the table are rows <span class="tex-span">0</span> and <span class="tex-span"><i>n</i> + 1</span> respectively. Also we define seats to the left of the table and to the right of the table to be column <span class="tex-span">0</span> and <span class="tex-span"><i>m</i> + 1</span>. Due to the conveyor belts direction restriction there are currently no way for a diner sitting in the row <span class="tex-span"><i>n</i> + 1</span> to be served.</p><p>Given the initial table, there will be <span class="tex-span"><i>q</i></span> events in order. There are two types of events:</p><ul> <li> "A <span class="tex-span"><i>x</i></span> <span class="tex-span"><i>y</i></span>" means, a piece of bread will appear at row <span class="tex-span"><i>x</i></span> and column <span class="tex-span"><i>y</i></span> (we will denote such position as <span class="tex-span">(<i>x</i>, <i>y</i>)</span>). The bread will follow the conveyor belt, until arriving at a seat of a diner. It is possible that the bread gets stuck in an infinite loop. Your task is to simulate the process, and output the final position of the bread, or determine that there will be an infinite loop. </li><li> "C <span class="tex-span"><i>x</i></span> <span class="tex-span"><i>y</i></span> <span class="tex-span"><i>c</i></span>" means that the type of the conveyor belt at <span class="tex-span">(<i>x</i>, <i>y</i>)</span> is changed to <span class="tex-span"><i>c</i></span>. </li></ul><p>Queries are performed separately meaning that even if the bread got stuck in an infinite loop, it won't affect further queries.</p></div><div class="input-specification"><p>The first line of input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>m</i> ≤ 10, 1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>), separated by a space.</p><p>Next <span class="tex-span"><i>n</i></span> lines, each line contains <span class="tex-span"><i>m</i></span> characters, describing the table. The characters can only be one of "<span class="tex-font-style-tt">&lt;^&gt;</span>".</p><p>Next <span class="tex-span"><i>q</i></span> lines, each line describes an event. The format is "<span class="tex-font-style-tt">C x y c</span>" or "<span class="tex-font-style-tt">A x y</span>" (Consecutive elements are separated by a space). It's guaranteed that <span class="tex-span">1 ≤ <i>x</i> ≤ <i>n</i>, 1 ≤ <i>y</i> ≤ <i>m</i></span>. <span class="tex-span"><i>c</i></span> is a character from the set "<span class="tex-font-style-tt">&lt;^&gt;</span>".</p><p>There are at most <span class="tex-span">10000</span> queries of "C" type.</p></div><div class="output-specification"><p>For each event of type "A", output two integers <span class="tex-span"><i>tx</i></span>, <span class="tex-span"><i>ty</i></span> in a line, separated by a space, denoting the destination of <span class="tex-span">(<i>x</i>, <i>y</i>)</span> is <span class="tex-span">(<i>tx</i>, <i>ty</i>)</span>.</p><p>If there is an infinite loop, you should output <span class="tex-span"><i>tx</i> = <i>ty</i> =  - 1</span>.</p></div>

## Input

<p>The first line of input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>m</i> ≤ 10, 1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>), separated by a space.</p><p>Next <span class="tex-span"><i>n</i></span> lines, each line contains <span class="tex-span"><i>m</i></span> characters, describing the table. The characters can only be one of "<span class="tex-font-style-tt">&lt;^&gt;</span>".</p><p>Next <span class="tex-span"><i>q</i></span> lines, each line describes an event. The format is "<span class="tex-font-style-tt">C x y c</span>" or "<span class="tex-font-style-tt">A x y</span>" (Consecutive elements are separated by a space). It's guaranteed that <span class="tex-span">1 ≤ <i>x</i> ≤ <i>n</i>, 1 ≤ <i>y</i> ≤ <i>m</i></span>. <span class="tex-span"><i>c</i></span> is a character from the set "<span class="tex-font-style-tt">&lt;^&gt;</span>".</p><p>There are at most <span class="tex-span">10000</span> queries of "C" type.</p>

## Output

<p>For each event of type "A", output two integers <span class="tex-span"><i>tx</i></span>, <span class="tex-span"><i>ty</i></span> in a line, separated by a space, denoting the destination of <span class="tex-span">(<i>x</i>, <i>y</i>)</span> is <span class="tex-span">(<i>tx</i>, <i>ty</i>)</span>.</p><p>If there is an infinite loop, you should output <span class="tex-span"><i>tx</i> = <i>ty</i> =  - 1</span>.</p>





```input1
2 2 3
&gt;&gt;
^^
A 2 1
C 1 2 &lt;
A 2 1

```




```input2
4 5 7
&gt;&lt;&lt;^&lt;
^&lt;^^&gt;
&gt;&gt;&gt;^&gt;
&gt;^&gt;&gt;^
A 3 1
A 2 2
C 1 4 &lt;
A 3 1
C 1 2 ^
A 3 1
A 2 2
```




```output1
1 3
-1 -1

```




```output2
0 4
-1 -1
-1 -1
0 2
0 2

```



## Note

<p>For the first sample:</p><p>If the bread goes from <span class="tex-span">(2, 1)</span>, it will go out of the table at <span class="tex-span">(1, 3)</span>.</p><p>After changing the conveyor belt of <span class="tex-span">(1, 2)</span> to "<span class="tex-font-style-tt">&lt;</span>", when the bread goes from <span class="tex-span">(2, 1)</span> again, it will get stuck at "<span class="tex-font-style-tt">&gt;&lt;</span>", so output is <span class="tex-span">( - 1,  - 1)</span>.</p>
