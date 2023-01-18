## Description

<div><p>Nastya owns too many arrays now, so she wants to delete the least important of them. However, she discovered that this array is magic! Nastya now knows that the array has the following properties:</p><ul> <li> In one second we can add an arbitrary (possibly negative) integer to all elements of the array that are not equal to zero. </li><li> When all elements of the array become equal to zero, the array explodes. </li></ul><p>Nastya is always busy, so she wants to explode the array as fast as possible. Compute the minimum time in which the array can be exploded.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the size of the array.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">5</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>) — the elements of the array.</p></div><div class="output-specification"><p>Print a single integer — the minimum number of seconds needed to make all elements of the array equal to zero.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the size of the array.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">5</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>) — the elements of the array.</p>

## Output

<p>Print a single integer — the minimum number of seconds needed to make all elements of the array equal to zero.</p>





```input1
5
1 1 1 1 1

```




```input2
3
2 0 -1

```




```input3
4
5 -6 -5 1

```




```output1
1

```




```output2
2

```




```output3
4

```



## Note

<p>In the first example you can add <span class="tex-span"> - 1</span> to all non-zero elements in one second and make them equal to zero.</p><p>In the second example you can add <span class="tex-span"> - 2</span> on the first second, then the array becomes equal to <span class="tex-span">[0, 0,  - 3]</span>. On the second second you can add <span class="tex-span">3</span> to the third (the only non-zero) element.</p>
