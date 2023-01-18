## Description

<div><p>Watchmen are in a danger and Doctor Manhattan together with his friend Daniel Dreiberg should warn them as soon as possible. There are <span class="tex-span"><i>n</i></span> watchmen on a plane, the <span class="tex-span"><i>i</i></span>-th watchman is located at point <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span>.</p><p>They need to arrange a plan, but there are some difficulties on their way. As you know, Doctor Manhattan considers the distance between watchmen <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> to be <span class="tex-span">|<i>x</i><sub class="lower-index"><i>i</i></sub> - <i>x</i><sub class="lower-index"><i>j</i></sub>| + |<i>y</i><sub class="lower-index"><i>i</i></sub> - <i>y</i><sub class="lower-index"><i>j</i></sub>|</span>. Daniel, as an ordinary person, calculates the distance using the formula <img align="middle" class="tex-formula" src="file://XYgxOti0.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>The success of the operation relies on the number of pairs <span class="tex-span">(<i>i</i>, <i>j</i>)</span> (<span class="tex-span">1 ≤ <i>i</i> &lt; <i>j</i> ≤ <i>n</i></span>), such that the distance between watchman <span class="tex-span"><i>i</i></span> and watchmen <span class="tex-span"><i>j</i></span> calculated by Doctor Manhattan is equal to the distance between them calculated by Daniel. You were asked to compute the number of such pairs.</p></div><div class="input-specification"><p>The first line of the input contains the single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the number of watchmen.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">|<i>x</i><sub class="lower-index"><i>i</i></sub>|, |<i>y</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">9</sup></span>).</p><p>Some positions may coincide.</p></div><div class="output-specification"><p>Print the number of pairs of watchmen such that the distance between them calculated by Doctor Manhattan is equal to the distance calculated by Daniel.</p></div>

## Input

<p>The first line of the input contains the single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the number of watchmen.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">|<i>x</i><sub class="lower-index"><i>i</i></sub>|, |<i>y</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">9</sup></span>).</p><p>Some positions may coincide.</p>

## Output

<p>Print the number of pairs of watchmen such that the distance between them calculated by Doctor Manhattan is equal to the distance calculated by Daniel.</p>





```input1
3
1 1
7 5
1 5

```




```input2
6
0 0
0 1
0 2
-1 1
0 1
1 1

```




```output1
2

```




```output2
11

```



## Note

<p>In the first sample, the distance between watchman <span class="tex-span">1</span> and watchman <span class="tex-span">2</span> is equal to <span class="tex-span">|1 - 7| + |1 - 5| = 10</span> for Doctor Manhattan and <img align="middle" class="tex-formula" src="file://b9TZU8c6.png" style="max-width: 100.0%;max-height: 100.0%;"> for Daniel. For pairs <span class="tex-span">(1, 1)</span>, <span class="tex-span">(1, 5)</span> and <span class="tex-span">(7, 5)</span>, <span class="tex-span">(1, 5)</span> Doctor Manhattan and Daniel will calculate the same distances.</p>
