## Description

<div><p>In the evening, after the contest Ilya was bored, and he really felt like maximizing. He remembered that he had a set of <span class="tex-span"><i>n</i></span> sticks and an instrument. Each stick is characterized by its length <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Ilya decided to make a rectangle from the sticks. And due to his whim, he decided to make rectangles in such a way that maximizes their total area. Each stick is used in making at most one rectangle, it is possible that some of sticks remain unused. Bending sticks is not allowed.</p><p>Sticks with lengths <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">3</sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index">4</sub></span> can make a rectangle if the following properties are observed:</p><ul> <li> <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> ≤ <i>a</i><sub class="lower-index">2</sub> ≤ <i>a</i><sub class="lower-index">3</sub> ≤ <i>a</i><sub class="lower-index">4</sub></span> </li><li> <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> = <i>a</i><sub class="lower-index">2</sub></span> </li><li> <span class="tex-span"><i>a</i><sub class="lower-index">3</sub> = <i>a</i><sub class="lower-index">4</sub></span> </li></ul><p>A rectangle can be made of sticks with lengths of, for example, <span class="tex-span">3&nbsp;3&nbsp;3&nbsp;3</span> or <span class="tex-span">2&nbsp;2&nbsp;4&nbsp;4</span>. A rectangle cannot be made of, for example, sticks <span class="tex-span">5&nbsp;5&nbsp;5&nbsp;7</span>.</p><p>Ilya also has an instrument which can reduce the length of the sticks. The sticks are made of a special material, so the length of each stick can be reduced by at most one. For example, a stick with length <span class="tex-span">5</span> can either stay at this length or be transformed into a stick of length <span class="tex-span">4</span>.</p><p>You have to answer the question — what maximum total area of the rectangles can Ilya get with a file if makes rectangles from the available sticks?</p></div><div class="input-specification"><p>The first line of the input contains a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;—&nbsp;the number of the available sticks.</p><p>The second line of the input contains <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">2 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;—&nbsp;the lengths of the sticks.</p></div><div class="output-specification"><p>The first line of the output must contain a single non-negative integer&nbsp;—&nbsp;the maximum total area of the rectangles that Ilya can make from the available sticks.</p></div>

## Input

<p>The first line of the input contains a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;—&nbsp;the number of the available sticks.</p><p>The second line of the input contains <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">2 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;—&nbsp;the lengths of the sticks.</p>

## Output

<p>The first line of the output must contain a single non-negative integer&nbsp;—&nbsp;the maximum total area of the rectangles that Ilya can make from the available sticks.</p>





```input1
4
2 4 4 2

```




```input2
4
2 2 3 5

```




```input3
4
100003 100004 100005 100006

```




```output1
8

```




```output2
0

```




```output3
10000800015

```


