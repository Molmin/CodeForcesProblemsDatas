## Description

<div><p>Kyoya Ootori has a bag with <span class="tex-span"><i>n</i></span> colored balls that are colored with <span class="tex-span"><i>k</i></span> different colors. The colors are labeled from <span class="tex-span">1</span> to <span class="tex-span"><i>k</i></span>. Balls of the same color are indistinguishable. He draws balls from the bag one by one until the bag is empty. He noticed that he drew the last ball of color <span class="tex-span"><i>i</i></span> before drawing the last ball of color <span class="tex-span"><i>i</i> + 1</span> for all <span class="tex-span"><i>i</i></span> from <span class="tex-span">1</span> to <span class="tex-span"><i>k</i> - 1</span>. Now he wonders how many different ways this can happen. </p></div><div class="input-specification"><p>The first line of input will have one integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 1000</span>) the number of colors.</p><p>Then, <span class="tex-span"><i>k</i></span> lines will follow. The <span class="tex-span"><i>i</i></span>-th line will contain <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>, the number of balls of the <span class="tex-span"><i>i</i></span>-th color (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>).</p><p>The total number of balls doesn't exceed 1000.</p></div><div class="output-specification"><p>A single integer, the number of ways that Kyoya can draw the balls from the bag as described in the statement, modulo <span class="tex-span">1 000 000 007</span>. </p></div>

## Input

<p>The first line of input will have one integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 1000</span>) the number of colors.</p><p>Then, <span class="tex-span"><i>k</i></span> lines will follow. The <span class="tex-span"><i>i</i></span>-th line will contain <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>, the number of balls of the <span class="tex-span"><i>i</i></span>-th color (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>).</p><p>The total number of balls doesn't exceed 1000.</p>

## Output

<p>A single integer, the number of ways that Kyoya can draw the balls from the bag as described in the statement, modulo <span class="tex-span">1 000 000 007</span>. </p>





```input1
3
2
2
1

```




```input2
4
1
2
3
4

```




```output1
3

```




```output2
1680

```



## Note

<p>In the first sample, we have 2 balls of color 1, 2 balls of color 2, and 1 ball of color 3. The three ways for Kyoya are: </p><pre class="verbatim"><br>1 2 1 2 3<br>1 1 2 2 3<br>2 1 1 2 3<br></pre>
