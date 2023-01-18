## Description

<div><p>An infinitely long railway has a train consisting of <span class="tex-span"><i>n</i></span> cars, numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> (the numbers of all the cars are distinct) and positioned in arbitrary order. David Blaine wants to sort the railway cars in the order of increasing numbers. In one move he can make one of the cars disappear from its place and teleport it either to the beginning of the train, or to the end of the train, at his desire. What is the minimum number of actions David Blaine needs to perform in order to sort the train?</p></div><div class="input-specification"><p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of cars in the train. </p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> ≠ <i>p</i><sub class="lower-index"><i>j</i></sub></span> if <span class="tex-span"><i>i</i> ≠ <i>j</i></span>)&nbsp;— the sequence of the numbers of the cars in the train.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the minimum number of actions needed to sort the railway cars.</p></div>

## Input

<p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of cars in the train. </p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> ≠ <i>p</i><sub class="lower-index"><i>j</i></sub></span> if <span class="tex-span"><i>i</i> ≠ <i>j</i></span>)&nbsp;— the sequence of the numbers of the cars in the train.</p>

## Output

<p>Print a single integer&nbsp;— the minimum number of actions needed to sort the railway cars.</p>





```input1
5
4 1 2 5 3

```




```input2
4
4 1 3 2

```




```output1
2

```




```output2
2

```



## Note

<p>In the first sample you need first to teleport the <span class="tex-span">4</span>-th car, and then the <span class="tex-span">5</span>-th car to the end of the train.</p>
