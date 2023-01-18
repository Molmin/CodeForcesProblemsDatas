## Description

<div><p>Artem has an array of <span class="tex-span"><i>n</i></span> positive integers. Artem decided to play with it. The game consists of <span class="tex-span"><i>n</i></span> moves. Each move goes like this. Artem chooses some element of the array and removes it. For that, he gets <span class="tex-span"><i>min</i>(<i>a</i>, <i>b</i>)</span> points, where <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> are numbers that were adjacent with the removed number. If the number doesn't have an adjacent number to the left or right, Artem doesn't get any points. </p><p>After the element is removed, the two parts of the array glue together resulting in the new array that Artem continues playing with. Borya wondered what maximum total number of points Artem can get as he plays this game.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup>)</span> — the number of elements in the array. The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup>)</span> — the values of the array elements.</p></div><div class="output-specification"><p>In a single line print a single integer — the maximum number of points Artem can get.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup>)</span> — the number of elements in the array. The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup>)</span> — the values of the array elements.</p>

## Output

<p>In a single line print a single integer — the maximum number of points Artem can get.</p>





```input1
5
3 1 5 2 6

```




```input2
5
1 2 3 4 5

```




```input3
5
1 100 101 100 1

```




```output1
11

```




```output2
6

```




```output3
102

```


