## Description

<div><p>Dima has a hamsters farm. Soon <span class="tex-span"><i>N</i></span> hamsters will grow up on it and Dima will sell them in a city nearby.</p><p>Hamsters should be transported in boxes. If some box is not completely full, the hamsters in it are bored, that's why each box should be completely full with hamsters.</p><p>Dima can buy boxes at a factory. The factory produces boxes of <span class="tex-span"><i>K</i></span> kinds, boxes of the <span class="tex-span"><i>i</i></span>-th kind can contain in themselves <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> hamsters. Dima can buy any amount of boxes, but he should buy boxes of only one kind to get a wholesale discount.</p><p>Of course, Dima would buy boxes in such a way that each box can be completely filled with hamsters and transported to the city. If there is no place for some hamsters, Dima will leave them on the farm.</p><p>Find out how many boxes and of which type should Dima buy to transport maximum number of hamsters.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>N</i></span> and <span class="tex-span"><i>K</i></span> (<span class="tex-span">0 ≤ <i>N</i> ≤ 10<sup class="upper-index">18</sup></span>, <span class="tex-span">1 ≤ <i>K</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of hamsters that will grow up on Dima's farm and the number of types of boxes that the factory produces.</p><p>The second line contains <span class="tex-span"><i>K</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>K</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">18</sup></span> for all <span class="tex-span"><i>i</i></span>)&nbsp;— the capacities of boxes.</p></div><div class="output-specification"><p>Output two integers: the type of boxes that Dima should buy and the number of boxes of that type Dima should buy. Types of boxes are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>K</i></span> in the order they are given in input.</p><p>If there are many correct answers, output any of them.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>N</i></span> and <span class="tex-span"><i>K</i></span> (<span class="tex-span">0 ≤ <i>N</i> ≤ 10<sup class="upper-index">18</sup></span>, <span class="tex-span">1 ≤ <i>K</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of hamsters that will grow up on Dima's farm and the number of types of boxes that the factory produces.</p><p>The second line contains <span class="tex-span"><i>K</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>K</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">18</sup></span> for all <span class="tex-span"><i>i</i></span>)&nbsp;— the capacities of boxes.</p>

## Output

<p>Output two integers: the type of boxes that Dima should buy and the number of boxes of that type Dima should buy. Types of boxes are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>K</i></span> in the order they are given in input.</p><p>If there are many correct answers, output any of them.</p>





```input1
19 3
5 4 10

```




```input2
28 3
5 6 30

```




```output1
2 4

```




```output2
1 5

```


