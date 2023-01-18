## Description

<div><p>Everybody knows of <a href="https://en.wikipedia.org/wiki/Spaghetti_sort">spaghetti sort</a>. You decided to implement an analog sorting algorithm yourself, but as you survey your pantry you realize you're out of spaghetti! The only type of pasta you have is ravioli, but you are not going to let this stop you...</p><p>You come up with the following algorithm. For each number in the array <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, build a stack of <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> ravioli. The image shows the stack for <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = 4</span>.</p><center> <img class="tex-graphics" src="file://16TDqvSS.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Arrange the stacks in one row in the order in which the corresponding numbers appear in the input array. Find the tallest one (if there are several stacks of maximal height, use the leftmost one). Remove it and add its height to the end of the output array. Shift the stacks in the row so that there is no gap between them. Repeat the procedure until all stacks have been removed.</p><p>At first you are very happy with your algorithm, but as you try it on more inputs you realize that it doesn't always produce the right sorted array. Turns out when two stacks of ravioli are next to each other (at any step of the process) and differ in height by two or more, the top ravioli of the taller stack slides down on top of the lower stack.</p><p>Given an input array, figure out whether the described algorithm will sort it correctly.</p></div><div class="input-specification"><p>The first line of input contains a single number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10</span>) — the size of the array.</p><p>The second line of input contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the elements of the array.</p></div><div class="output-specification"><p>Output "YES" if the array can be sorted using the described procedure and "NO" if it can not.</p></div>

## Input

<p>The first line of input contains a single number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10</span>) — the size of the array.</p><p>The second line of input contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the elements of the array.</p>

## Output

<p>Output "YES" if the array can be sorted using the described procedure and "NO" if it can not.</p>





```input1
3
1 2 3

```




```input2
3
3 1 2

```




```output1
YES

```




```output2
NO

```



## Note

<p>In the second example the array will change even before the tallest stack is chosen for the first time: ravioli from stack of height 3 will slide on the stack of height 1, and the algorithm will output an array <span class="tex-span">{2, 2, 2}</span>.</p>
