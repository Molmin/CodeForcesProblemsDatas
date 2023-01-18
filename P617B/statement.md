## Description

<div><p>Bob loves everything sweet. His favorite chocolate bar consists of pieces, each piece may contain a nut. Bob wants to break the bar of chocolate into multiple pieces so that each part would contain <span class="tex-font-style-bf">exactly</span> one nut and any break line goes between two adjacent pieces.</p><p>You are asked to calculate the number of ways he can do it. Two ways to break chocolate are considered distinct if one of them contains a break between some two adjacent pieces and the other one doesn't. </p><p>Please note, that if Bob doesn't make any breaks, all the bar will form one piece and it still has to have exactly one nut.</p></div><div class="input-specification"><p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the number of pieces in the chocolate bar.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1</span>), where <span class="tex-span">0</span> represents a piece without the nut and <span class="tex-span">1</span> stands for a piece with the nut.</p></div><div class="output-specification"><p>Print the number of ways to break the chocolate into multiple parts so that each part would contain exactly one nut.</p></div>

## Input

<p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the number of pieces in the chocolate bar.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1</span>), where <span class="tex-span">0</span> represents a piece without the nut and <span class="tex-span">1</span> stands for a piece with the nut.</p>

## Output

<p>Print the number of ways to break the chocolate into multiple parts so that each part would contain exactly one nut.</p>





```input1
3
0 1 0

```




```input2
5
1 0 1 0 1

```




```output1
1

```




```output2
4

```



## Note

<p>In the first sample there is exactly one nut, so the number of ways equals <span class="tex-span">1</span>&nbsp;— Bob shouldn't make any breaks.</p><p>In the second sample you can break the bar in four ways:</p><p><span class="tex-font-style-tt">10|10|1</span></p><p><span class="tex-font-style-tt">1|010|1</span></p><p><span class="tex-font-style-tt">10|1|01</span></p><p><span class="tex-font-style-tt">1|01|01</span></p>
