## Description

<div><p>Vanya and his friends are walking along the fence of height <span class="tex-span"><i>h</i></span> and they do not want the guard to notice them. In order to achieve this the height of each of the friends should not exceed <span class="tex-span"><i>h</i></span>. If the height of some person is greater than <span class="tex-span"><i>h</i></span> he can bend down and then he surely won't be noticed by the guard. The height of the <span class="tex-span"><i>i</i></span>-th person is equal to <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Consider the width of the person walking as usual to be equal to <span class="tex-span">1</span>, while the width of the bent person is equal to <span class="tex-span">2</span>. Friends want to talk to each other while walking, so they would like to walk in a single row. What is the minimum width of the road, such that friends can walk in a row and remain unattended by the guard?</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>h</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>h</i> ≤ 1000</span>)&nbsp;— the number of friends and the height of the fence, respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 2<i>h</i></span>), the <span class="tex-span"><i>i</i></span>-th of them is equal to the height of the <span class="tex-span"><i>i</i></span>-th person.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the minimum possible valid width of the road.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>h</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>h</i> ≤ 1000</span>)&nbsp;— the number of friends and the height of the fence, respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 2<i>h</i></span>), the <span class="tex-span"><i>i</i></span>-th of them is equal to the height of the <span class="tex-span"><i>i</i></span>-th person.</p>

## Output

<p>Print a single integer&nbsp;— the minimum possible valid width of the road.</p>





```input1
3 7
4 5 14

```




```input2
6 1
1 1 1 1 1 1

```




```input3
6 5
7 6 8 9 10 5

```




```output1
4

```




```output2
6

```




```output3
11

```



## Note

<p>In the first sample, only person number <span class="tex-span">3</span> must bend down, so the required width is equal to <span class="tex-span">1 + 1 + 2 = 4</span>.</p><p>In the second sample, all friends are short enough and no one has to bend, so the width <span class="tex-span">1 + 1 + 1 + 1 + 1 + 1 = 6</span> is enough.</p><p>In the third sample, all the persons have to bend, except the last one. The required minimum width of the road is equal to <span class="tex-span">2 + 2 + 2 + 2 + 2 + 1 = 11</span>.</p>
