## Description

<div><p>DZY owns <span class="tex-span">2<sup class="upper-index"><i>m</i></sup></span> islands near his home, numbered from <span class="tex-span">1</span> to <span class="tex-span">2<sup class="upper-index"><i>m</i></sup></span>. He loves building bridges to connect the islands. Every bridge he builds takes one day's time to walk across.</p><p>DZY has a strange rule of building the bridges. For every pair of islands <span class="tex-span"><i>u</i>, <i>v</i>&nbsp;(<i>u</i> ≠ <i>v</i>)</span>, he has built <span class="tex-span">2<sup class="upper-index"><i>k</i></sup></span> different bridges connecting them, where <img align="middle" class="tex-formula" src="file://sYxz4y6W.png" style="max-width: 100.0%;max-height: 100.0%;"> (<span class="tex-span"><i>a</i>|<i>b</i></span> means <span class="tex-span"><i>b</i></span> is divisible by <span class="tex-span"><i>a</i></span>). These bridges are bidirectional.</p><p>Also, DZY has built some bridges connecting his home with the islands. Specifically, there are <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> different bridges from his home to the <span class="tex-span"><i>i</i></span>-th island. These are one-way bridges, so after he leaves his home he will never come back.</p><p>DZY decides to go to the islands for sightseeing. At first he is at home. He chooses and walks across one of the bridges connecting with his home, and arrives at some island. After that, he will spend <span class="tex-span"><i>t</i></span> day(s) on the islands. Each day, he can choose to stay and rest, or to walk to another island across the bridge. It is allowed to stay at an island for more than one day. It's also allowed to cross one bridge more than once.</p><p>Suppose that right after the <span class="tex-span"><i>t</i></span>-th day DZY stands at the <span class="tex-span"><i>i</i></span>-th island. Let <span class="tex-span"><i>ans</i>[<i>i</i>]</span> be the number of ways for DZY to reach the <span class="tex-span"><i>i</i></span>-th island after <span class="tex-span"><i>t</i></span>-th day. Your task is to calculate <span class="tex-span"><i>ans</i>[<i>i</i>]</span> for each <span class="tex-span"><i>i</i></span> modulo <span class="tex-span">1051131</span>.</p></div><div class="input-specification"><p>To avoid huge input, we use the following way to generate the array <span class="tex-span"><i>a</i></span>. You are given the first <span class="tex-span"><i>s</i></span> elements of array: <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>s</i></sub></span>. All the other elements should be calculated by formula: <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = (101·<i>a</i><sub class="lower-index"><i>i</i> - <i>s</i></sub> + 10007)&nbsp;<i>mod</i>&nbsp;1051131</span> <span class="tex-span">(<i>s</i> &lt; <i>i</i> ≤ 2<sup class="upper-index"><i>m</i></sup>)</span>.</p><p>The first line contains three integers <span class="tex-span"><i>m</i>, <i>t</i>, <i>s</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 25;&nbsp;1 ≤ <i>t</i> ≤ 10<sup class="upper-index">18</sup>;&nbsp;1 ≤ <i>s</i> ≤ <i>min</i>(2<sup class="upper-index"><i>m</i></sup>, 10<sup class="upper-index">5</sup>))</span>.</p><p>The second line contains <span class="tex-span"><i>s</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>s</i></sub>&nbsp;(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup>)</span>.</p></div><div class="output-specification"><p>To avoid huge output, you only need to output xor-sum of all the answers for all <span class="tex-span"><i>i</i></span> modulo <span class="tex-span">1051131</span> <span class="tex-span">(1 ≤ <i>i</i> ≤ 2<sup class="upper-index"><i>m</i></sup>)</span>, i.e. <span class="tex-span">(<i>ans</i>[1]&nbsp;<i>mod</i>&nbsp;1051131)&nbsp;<i>xor</i>&nbsp;(<i>ans</i>[2]&nbsp;<i>mod</i>&nbsp;1051131)&nbsp;<i>xor</i>... <i>xor</i>&nbsp;(<i>ans</i>[<i>n</i>]&nbsp;<i>mod</i>&nbsp;1051131)</span>.</p></div>

## Input

<p>To avoid huge input, we use the following way to generate the array <span class="tex-span"><i>a</i></span>. You are given the first <span class="tex-span"><i>s</i></span> elements of array: <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>s</i></sub></span>. All the other elements should be calculated by formula: <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = (101·<i>a</i><sub class="lower-index"><i>i</i> - <i>s</i></sub> + 10007)&nbsp;<i>mod</i>&nbsp;1051131</span> <span class="tex-span">(<i>s</i> &lt; <i>i</i> ≤ 2<sup class="upper-index"><i>m</i></sup>)</span>.</p><p>The first line contains three integers <span class="tex-span"><i>m</i>, <i>t</i>, <i>s</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 25;&nbsp;1 ≤ <i>t</i> ≤ 10<sup class="upper-index">18</sup>;&nbsp;1 ≤ <i>s</i> ≤ <i>min</i>(2<sup class="upper-index"><i>m</i></sup>, 10<sup class="upper-index">5</sup>))</span>.</p><p>The second line contains <span class="tex-span"><i>s</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>s</i></sub>&nbsp;(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup>)</span>.</p>

## Output

<p>To avoid huge output, you only need to output xor-sum of all the answers for all <span class="tex-span"><i>i</i></span> modulo <span class="tex-span">1051131</span> <span class="tex-span">(1 ≤ <i>i</i> ≤ 2<sup class="upper-index"><i>m</i></sup>)</span>, i.e. <span class="tex-span">(<i>ans</i>[1]&nbsp;<i>mod</i>&nbsp;1051131)&nbsp;<i>xor</i>&nbsp;(<i>ans</i>[2]&nbsp;<i>mod</i>&nbsp;1051131)&nbsp;<i>xor</i>... <i>xor</i>&nbsp;(<i>ans</i>[<i>n</i>]&nbsp;<i>mod</i>&nbsp;1051131)</span>.</p>





```input1
2 1 4
1 1 1 2

```




```input2
3 5 6
389094 705719 547193 653800 947499 17024

```




```output1
1

```




```output2
556970

```



## Note

<p>In the first sample, <span class="tex-span"><i>ans</i> = [6, 7, 6, 6]</span>.</p><p>If he wants to be at island 1 after one day, he has 6 different ways:</p><ol> <li> home —&gt; 1 -(stay)-&gt; 1 </li><li> home —&gt; 2 —&gt; 1 </li><li> home —&gt; 3 —&gt; 1 </li><li> home —&gt; 3 —&gt; 1 (note that there are two different bridges between 1 and 3) </li><li> home —&gt; 4 —&gt; 1 </li><li> home —&gt; 4 —&gt; 1 (note that there are two different bridges from home to 4) </li></ol><p>In the second sample, <span class="tex-span">(<i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, <i>a</i><sub class="lower-index">3</sub>, <i>a</i><sub class="lower-index">4</sub>, <i>a</i><sub class="lower-index">5</sub>, <i>a</i><sub class="lower-index">6</sub>, <i>a</i><sub class="lower-index">7</sub>, <i>a</i><sub class="lower-index">8</sub>) = (389094, 705719, 547193, 653800, 947499, 17024, 416654, 861849)</span>, <span class="tex-span"><i>ans</i> = [235771, 712729, 433182, 745954, 139255, 935785, 620229, 644335]</span>.</p>
