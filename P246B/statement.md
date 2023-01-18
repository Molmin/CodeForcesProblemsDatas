## Description

<div><p>Polycarpus has an array, consisting of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. Polycarpus likes it when numbers in an array match. That's why he wants the array to have as many equal numbers as possible. For that Polycarpus performs the following operation multiple times:</p><ul> <li> he chooses two elements of the array <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span> <span class="tex-span">(<i>i</i> ≠ <i>j</i>)</span>; </li><li> he simultaneously increases number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> by <span class="tex-span">1</span> and decreases number <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span> by <span class="tex-span">1</span>, that is, executes <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = <i>a</i><sub class="lower-index"><i>i</i></sub> + 1</span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub> = <i>a</i><sub class="lower-index"><i>j</i></sub> - 1</span>. </li></ul><p>The given operation changes exactly two distinct array elements. Polycarpus can apply the described operation an infinite number of times. </p><p>Now he wants to know what maximum number of equal array elements he can get if he performs an arbitrary number of such operation. Help Polycarpus.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the array size. The second line contains space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">|<i>a</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">4</sup></span>) — the original array.</p></div><div class="output-specification"><p>Print a single integer — the maximum number of equal array elements he can get if he performs an arbitrary number of the given operation.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the array size. The second line contains space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">|<i>a</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">4</sup></span>) — the original array.</p>

## Output

<p>Print a single integer — the maximum number of equal array elements he can get if he performs an arbitrary number of the given operation.</p>





```input1
2
2 1

```




```input2
3
1 4 1

```




```output1
1

```




```output2
3

```


