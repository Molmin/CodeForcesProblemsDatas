## Description

<div><p>Molly Hooper has <span class="tex-span"><i>n</i></span> different kinds of chemicals arranged in a line. Each of the chemicals has an affection value, The <span class="tex-span"><i>i</i></span>-th of them has affection value <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Molly wants Sherlock to fall in love with her. She intends to do this by mixing a contiguous segment of chemicals together to make a love potion with total affection value as a non-negative <span class="tex-font-style-bf">integer</span> power of <span class="tex-span"><i>k</i></span>. Total affection value of a continuous segment of chemicals is the sum of affection values of each chemical in that segment.</p><p>Help her to do so in finding the total number of such segments.</p></div><div class="input-specification"><p>The first line of input contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span>, the number of chemicals and the number, such that the total affection value is a non-negative power of this number <span class="tex-span"><i>k</i></span>. (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ |<i>k</i>| ≤ 10</span>).</p><p>Next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— affection values of chemicals.</p></div><div class="output-specification"><p>Output a single integer&nbsp;— the number of valid segments.</p></div>

## Input

<p>The first line of input contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span>, the number of chemicals and the number, such that the total affection value is a non-negative power of this number <span class="tex-span"><i>k</i></span>. (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ |<i>k</i>| ≤ 10</span>).</p><p>Next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— affection values of chemicals.</p>

## Output

<p>Output a single integer&nbsp;— the number of valid segments.</p>





```input1
4 2
2 2 2 2

```




```input2
4 -3
3 -6 -3 12

```




```output1
8

```




```output2
3

```



## Note

<p>Do keep in mind that <span class="tex-span"><i>k</i><sup class="upper-index">0</sup> = 1</span>.</p><p>In the first sample, Molly can get following different affection values: </p><ul> <li><span class="tex-span">2</span>: segments <span class="tex-span">[1, 1]</span>, <span class="tex-span">[2, 2]</span>, <span class="tex-span">[3, 3]</span>, <span class="tex-span">[4, 4]</span>;<p> </p></li><li><span class="tex-span">4</span>: segments <span class="tex-span">[1, 2]</span>, <span class="tex-span">[2, 3]</span>, <span class="tex-span">[3, 4]</span>;<p> </p></li><li><span class="tex-span">6</span>: segments <span class="tex-span">[1, 3]</span>, <span class="tex-span">[2, 4]</span>;<p> </p></li><li><span class="tex-span">8</span>: segments <span class="tex-span">[1, 4]</span>. </li></ul><p>Out of these, <span class="tex-span">2</span>, <span class="tex-span">4</span> and <span class="tex-span">8</span> are powers of <span class="tex-span"><i>k</i> = 2</span>. Therefore, the answer is <span class="tex-span">8</span>.</p><p>In the second sample, Molly can choose segments <span class="tex-span">[1, 2]</span>, <span class="tex-span">[3, 3]</span>, <span class="tex-span">[3, 4]</span>.</p>
