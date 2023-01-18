## Description

<div><p>Vasya has an array <span class="tex-span"><i>a</i></span> consisting of positive integer numbers. Vasya wants to divide this array into two non-empty consecutive parts (the prefix and the suffix) so that the sum of all elements in the first part equals to the sum of elements in the second part. It is not always possible, so Vasya will move some element before dividing the array (Vasya will erase some element and insert it into an arbitrary position).</p><p><span class="tex-font-style-bf">Inserting an element in the same position he was erased from is also considered moving.</span></p><p>Can Vasya divide the array after choosing the right element to move and its new position?</p></div><div class="input-specification"><p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100000</span>) — the size of the array.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>... <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the elements of the array.</p></div><div class="output-specification"><p>Print <span class="tex-font-style-tt">YES</span> if Vasya can divide the array after moving one element. Otherwise print <span class="tex-font-style-tt">NO</span>.</p></div>

## Input

<p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100000</span>) — the size of the array.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>... <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the elements of the array.</p>

## Output

<p>Print <span class="tex-font-style-tt">YES</span> if Vasya can divide the array after moving one element. Otherwise print <span class="tex-font-style-tt">NO</span>.</p>





```input1
3
1 3 2

```




```input2
5
1 2 3 4 5

```




```input3
5
2 2 3 4 5

```




```output1
YES

```




```output2
NO

```




```output3
YES

```



## Note

<p>In the first example Vasya can move the second element to the end of the array.</p><p>In the second example no move can make the division possible.</p><p>In the third example Vasya can move the fourth element by one position to the left.</p>
