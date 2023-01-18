## Description

<div><p>Of course you have heard the famous task about Hanoi Towers, but did you know that there is a special factory producing the rings for this wonderful game? Once upon a time, the ruler of the ancient Egypt ordered the workers of Hanoi Factory to create as high tower as possible. They were not ready to serve such a strange order so they had to create this new tower using already produced rings.</p><p>There are <span class="tex-span"><i>n</i></span> rings in factory's stock. The <span class="tex-span"><i>i</i></span>-th ring has inner radius <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, outer radius <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and height <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span>. The goal is to select some subset of rings and arrange them such that the following conditions are satisfied:</p><ul> <li> Outer radiuses form a non-increasing sequence, i.e. one can put the <span class="tex-span"><i>j</i></span>-th ring on the <span class="tex-span"><i>i</i></span>-th ring only if <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub> ≤ <i>b</i><sub class="lower-index"><i>i</i></sub></span>. </li><li> Rings should not fall one into the the other. That means one can place ring <span class="tex-span"><i>j</i></span> on the ring <span class="tex-span"><i>i</i></span> only if <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub> &gt; <i>a</i><sub class="lower-index"><i>i</i></sub></span>. </li><li> The total height of all rings used should be maximum possible. </li></ul></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of rings in factory's stock.</p><p>The <span class="tex-span"><i>i</i></span>-th of the next <span class="tex-span"><i>n</i></span> lines contains three integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub> &gt; <i>a</i><sub class="lower-index"><i>i</i></sub></span>)&nbsp;— inner radius, outer radius and the height of the <span class="tex-span"><i>i</i></span>-th ring respectively.</p></div><div class="output-specification"><p>Print one integer&nbsp;— the maximum height of the tower that can be obtained.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of rings in factory's stock.</p><p>The <span class="tex-span"><i>i</i></span>-th of the next <span class="tex-span"><i>n</i></span> lines contains three integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub> &gt; <i>a</i><sub class="lower-index"><i>i</i></sub></span>)&nbsp;— inner radius, outer radius and the height of the <span class="tex-span"><i>i</i></span>-th ring respectively.</p>

## Output

<p>Print one integer&nbsp;— the maximum height of the tower that can be obtained.</p>





```input1
3
1 5 1
2 6 2
3 7 3

```




```input2
4
1 2 1
1 3 3
4 6 2
5 7 1

```




```output1
6

```




```output2
4

```



## Note

<p>In the first sample, the optimal solution is to take all the rings and put them on each other in order <span class="tex-span">3</span>, <span class="tex-span">2</span>, <span class="tex-span">1</span>.</p><p>In the second sample, one can put the ring <span class="tex-span">3</span> on the ring <span class="tex-span">4</span> and get the tower of height <span class="tex-span">3</span>, or put the ring <span class="tex-span">1</span> on the ring <span class="tex-span">2</span> and get the tower of height <span class="tex-span">4</span>.</p>
