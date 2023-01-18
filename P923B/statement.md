## Description

<div><p>Alice likes snow a lot! Unfortunately, this year's winter is already over, and she can't expect to have any more of it. Bob has thus bought her a gift&nbsp;— a large snow maker. He plans to make some amount of snow every day. On day <span class="tex-span"><i>i</i></span> he will make a pile of snow of volume <span class="tex-span"><i>V</i><sub class="lower-index"><i>i</i></sub></span> and put it in her garden.</p><p>Each day, every pile will shrink a little due to melting. More precisely, when the temperature on a given day is <span class="tex-span"><i>T</i><sub class="lower-index"><i>i</i></sub></span>, each pile will reduce its volume by <span class="tex-span"><i>T</i><sub class="lower-index"><i>i</i></sub></span>. If this would reduce the volume of a pile to or below zero, it disappears forever. All snow piles are independent of each other. </p><p>Note that the pile made on day <span class="tex-span"><i>i</i></span> already loses part of its volume on the same day. In an extreme case, this may mean that there are no piles left at the end of a particular day.</p><p>You are given the initial pile sizes and the temperature on each day. Determine the total volume of snow melted on each day. </p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>N</i></span> (<span class="tex-span">1 ≤ <i>N</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of days. </p><p>The second line contains <span class="tex-span"><i>N</i></span> integers <span class="tex-span"><i>V</i><sub class="lower-index">1</sub>, <i>V</i><sub class="lower-index">2</sub>, ..., <i>V</i><sub class="lower-index"><i>N</i></sub></span> (<span class="tex-span">0 ≤ <i>V</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>V</i><sub class="lower-index"><i>i</i></sub></span> is the initial size of a snow pile made on the day <span class="tex-span"><i>i</i></span>.</p><p>The third line contains <span class="tex-span"><i>N</i></span> integers <span class="tex-span"><i>T</i><sub class="lower-index">1</sub>, <i>T</i><sub class="lower-index">2</sub>, ..., <i>T</i><sub class="lower-index"><i>N</i></sub></span> (<span class="tex-span">0 ≤ <i>T</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>T</i><sub class="lower-index"><i>i</i></sub></span> is the temperature on the day <span class="tex-span"><i>i</i></span>.</p></div><div class="output-specification"><p>Output a single line with <span class="tex-span"><i>N</i></span> integers, where the <span class="tex-span"><i>i</i></span>-th integer represents the total volume of snow melted on day <span class="tex-span"><i>i</i></span>.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>N</i></span> (<span class="tex-span">1 ≤ <i>N</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of days. </p><p>The second line contains <span class="tex-span"><i>N</i></span> integers <span class="tex-span"><i>V</i><sub class="lower-index">1</sub>, <i>V</i><sub class="lower-index">2</sub>, ..., <i>V</i><sub class="lower-index"><i>N</i></sub></span> (<span class="tex-span">0 ≤ <i>V</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>V</i><sub class="lower-index"><i>i</i></sub></span> is the initial size of a snow pile made on the day <span class="tex-span"><i>i</i></span>.</p><p>The third line contains <span class="tex-span"><i>N</i></span> integers <span class="tex-span"><i>T</i><sub class="lower-index">1</sub>, <i>T</i><sub class="lower-index">2</sub>, ..., <i>T</i><sub class="lower-index"><i>N</i></sub></span> (<span class="tex-span">0 ≤ <i>T</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>T</i><sub class="lower-index"><i>i</i></sub></span> is the temperature on the day <span class="tex-span"><i>i</i></span>.</p>

## Output

<p>Output a single line with <span class="tex-span"><i>N</i></span> integers, where the <span class="tex-span"><i>i</i></span>-th integer represents the total volume of snow melted on day <span class="tex-span"><i>i</i></span>.</p>





```input1
3
10 10 5
5 7 2

```




```input2
5
30 25 20 15 10
9 10 12 4 13

```




```output1
5 12 4

```




```output2
9 20 35 11 25

```



## Note

<p>In the first sample, Bob first makes a snow pile of volume 10, which melts to the size of 5 on the same day. On the second day, he makes another pile of size 10. Since it is a bit warmer than the day before, the first pile disappears completely while the second pile shrinks to 3. At the end of the second day, he has only a single pile of size 3. On the third day he makes a smaller pile than usual, but as the temperature dropped too, both piles survive till the end of the day.</p>
