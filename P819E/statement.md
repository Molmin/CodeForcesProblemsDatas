## Description

<div><p>In order to fly to the Moon Mister B just needs to solve the following problem.</p><p>There is a complete indirected graph with <span class="tex-span"><i>n</i></span> vertices. You need to cover it with several simple cycles of length <span class="tex-span">3</span> and <span class="tex-span">4</span> so that each edge is in exactly <span class="tex-span">2</span> cycles.</p><p>We are sure that Mister B will solve the problem soon and will fly to the Moon. Will you?</p></div><div class="input-specification"><p>The only line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 300</span>).</p></div><div class="output-specification"><p>If there is no answer, print <span class="tex-font-style-tt">-1</span>.</p><p>Otherwise, in the first line print <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i><sup class="upper-index">2</sup></span>)&nbsp;— the number of cycles in your solution.</p><p>In each of the next <span class="tex-span"><i>k</i></span> lines print description of one cycle in the following format: first print integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">3 ≤ <i>m</i> ≤ 4</span>)&nbsp;— the length of the cycle, then print <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>v</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">2</sub>, ..., <i>v</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— the vertices in the cycle in the traverse order. Each edge should be in exactly two cycles.</p></div>

## Input

<p>The only line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 300</span>).</p>

## Output

<p>If there is no answer, print <span class="tex-font-style-tt">-1</span>.</p><p>Otherwise, in the first line print <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i><sup class="upper-index">2</sup></span>)&nbsp;— the number of cycles in your solution.</p><p>In each of the next <span class="tex-span"><i>k</i></span> lines print description of one cycle in the following format: first print integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">3 ≤ <i>m</i> ≤ 4</span>)&nbsp;— the length of the cycle, then print <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>v</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">2</sub>, ..., <i>v</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— the vertices in the cycle in the traverse order. Each edge should be in exactly two cycles.</p>





```input1
3

```




```input2
5

```




```output1
2
3 1 2 3
3 1 2 3

```




```output2
6
3 5 4 2
3 3 1 5
4 4 5 2 3
4 4 3 2 1
3 4 2 1
3 3 1 5

```


