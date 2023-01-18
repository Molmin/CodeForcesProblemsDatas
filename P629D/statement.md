## Description

<div><p>As you know, every birthday party has a cake! This time, Babaei is going to prepare the very special birthday party's cake.</p><p><span class="tex-font-style-it">Simple cake</span> is a cylinder of some radius and height. The volume of the simple cake is equal to the volume of corresponding cylinder. Babaei has <span class="tex-span"><i>n</i></span> simple cakes and he is going to make a <span class="tex-font-style-it">special cake</span> placing some cylinders on each other.</p><p>However, there are some additional culinary restrictions. The cakes are numbered in such a way that the cake number <span class="tex-span"><i>i</i></span> can be placed only on the table or on some cake number <span class="tex-span"><i>j</i></span> where <span class="tex-span"><i>j</i> &lt; <i>i</i></span>. Moreover, in order to impress friends Babaei will put the cake <span class="tex-span"><i>i</i></span> on top of the cake <span class="tex-span"><i>j</i></span> only if the volume of the cake <span class="tex-span"><i>i</i></span> is strictly greater than the volume of the cake <span class="tex-span"><i>j</i></span>.</p><p>Babaei wants to prepare a birthday cake that has a maximum possible total volume. Help him find this value.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000)</span>&nbsp;— the number of simple cakes Babaei has.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub>, <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 10 000</span>), giving the radius and height of the <span class="tex-span"><i>i</i></span>-th cake.</p></div><div class="output-specification"><p>Print the maximum volume of the cake that Babaei can make. Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct, if <img align="middle" class="tex-formula" src="file://ddWmkOLI.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000)</span>&nbsp;— the number of simple cakes Babaei has.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub>, <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 10 000</span>), giving the radius and height of the <span class="tex-span"><i>i</i></span>-th cake.</p>

## Output

<p>Print the maximum volume of the cake that Babaei can make. Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct, if <img align="middle" class="tex-formula" src="file://ddWmkOLI.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
2
100 30
40 10

```




```input2
4
1 1
9 7
1 4
10 7

```




```output1
942477.796077000

```




```output2
3983.539484752

```



## Note

<p>In first sample, the optimal way is to choose the cake number <span class="tex-span">1</span>.</p><p>In second sample, the way to get the maximum volume is to use cakes with indices <span class="tex-span">1</span>, <span class="tex-span">2</span> and <span class="tex-span">4</span>.</p>
