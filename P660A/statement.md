## Description

<div><p>You are given an array of <span class="tex-span"><i>n</i></span> elements, you must make it a co-prime array in as few moves as possible.</p><p>In each move you can insert any positive integral number you want not greater than <span class="tex-span">10<sup class="upper-index">9</sup></span> in any place in the array.</p><p>An array is co-prime if any two adjacent numbers of it are co-prime.</p><p>In the number theory, two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> are said to be co-prime if the only positive integer that divides both of them is <span class="tex-span">1</span>.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>) — the number of elements in the given array.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the elements of the array <span class="tex-span"><i>a</i></span>.</p></div><div class="output-specification"><p>Print integer <span class="tex-span"><i>k</i></span> on the first line — the least number of elements needed to add to the array <span class="tex-span"><i>a</i></span> to make it co-prime.</p><p>The second line should contain <span class="tex-span"><i>n</i> + <i>k</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span> — the elements of the array <span class="tex-span"><i>a</i></span> after adding <span class="tex-span"><i>k</i></span> elements to it. Note that the new array should be co-prime, so any two adjacent values should be co-prime. Also the new array should be got from the original array <span class="tex-span"><i>a</i></span> by adding <span class="tex-span"><i>k</i></span> elements to it.</p><p>If there are multiple answers you can print any one of them.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>) — the number of elements in the given array.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the elements of the array <span class="tex-span"><i>a</i></span>.</p>

## Output

<p>Print integer <span class="tex-span"><i>k</i></span> on the first line — the least number of elements needed to add to the array <span class="tex-span"><i>a</i></span> to make it co-prime.</p><p>The second line should contain <span class="tex-span"><i>n</i> + <i>k</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span> — the elements of the array <span class="tex-span"><i>a</i></span> after adding <span class="tex-span"><i>k</i></span> elements to it. Note that the new array should be co-prime, so any two adjacent values should be co-prime. Also the new array should be got from the original array <span class="tex-span"><i>a</i></span> by adding <span class="tex-span"><i>k</i></span> elements to it.</p><p>If there are multiple answers you can print any one of them.</p>





```input1
3
2 7 28

```




```output1
1
2 7 9 28

```


