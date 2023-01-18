## Description

<div><p>Professor GukiZ has two arrays of integers, <span class="tex-font-style-tt">a</span> and <span class="tex-font-style-tt">b</span>. Professor wants to make the sum of the elements in the array <span class="tex-font-style-tt">a</span> <span class="tex-span"><i>s</i><sub class="lower-index"><i>a</i></sub></span> as close as possible to the sum of the elements in the array <span class="tex-font-style-tt">b</span> <span class="tex-span"><i>s</i><sub class="lower-index"><i>b</i></sub></span>. So he wants to minimize the value <span class="tex-span"><i>v</i> = |<i>s</i><sub class="lower-index"><i>a</i></sub> - <i>s</i><sub class="lower-index"><i>b</i></sub>|</span>.</p><p>In one operation professor can swap some element from the array <span class="tex-font-style-tt">a</span> and some element from the array <span class="tex-font-style-tt">b</span>. For example if the array <span class="tex-font-style-tt">a</span> is <span class="tex-span">[5, 1, 3, 2, 4]</span> and the array <span class="tex-font-style-tt">b</span> is <span class="tex-span">[3, 3, 2]</span> professor can swap the element <span class="tex-span">5</span> from the array <span class="tex-font-style-tt">a</span> and the element <span class="tex-span">2</span> from the array <span class="tex-font-style-tt">b</span> and get the new array <span class="tex-font-style-tt">a</span> <span class="tex-span">[2, 1, 3, 2, 4]</span> and the new array <span class="tex-font-style-tt">b</span> <span class="tex-span">[3, 3, 5]</span>.</p><p>Professor doesn't want to make more than two swaps. Find the minimal value <span class="tex-span"><i>v</i></span> and some sequence of no more than two swaps that will lead to the such value <span class="tex-span"><i>v</i></span>. Professor makes swaps one by one, each new swap he makes with the new arrays <span class="tex-font-style-tt">a</span> and <span class="tex-font-style-tt">b</span>.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2000</span>) — the number of elements in the array <span class="tex-font-style-tt">a</span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the elements of the array <span class="tex-font-style-tt">a</span>.</p><p>The third line contains integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 2000</span>) — the number of elements in the array <span class="tex-font-style-tt">b</span>.</p><p>The fourth line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>b</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the elements of the array <span class="tex-font-style-tt">b</span>.</p></div><div class="output-specification"><p>In the first line print the minimal value <span class="tex-span"><i>v</i> = |<i>s</i><sub class="lower-index"><i>a</i></sub> - <i>s</i><sub class="lower-index"><i>b</i></sub>|</span> that can be got with no more than two swaps.</p><p>The second line should contain the number of swaps <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 2</span>).</p><p>Each of the next <span class="tex-span"><i>k</i></span> lines should contain two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>p</i></sub>, <i>y</i><sub class="lower-index"><i>p</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>p</i></sub> ≤ <i>n</i>, 1 ≤ <i>y</i><sub class="lower-index"><i>p</i></sub> ≤ <i>m</i></span>) — the index of the element in the array <span class="tex-font-style-tt">a</span> and the index of the element in the array <span class="tex-font-style-tt">b</span> in the <span class="tex-span"><i>p</i></span>-th swap.</p><p>If there are several optimal solutions print any of them. Print the swaps in order the professor did them.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2000</span>) — the number of elements in the array <span class="tex-font-style-tt">a</span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the elements of the array <span class="tex-font-style-tt">a</span>.</p><p>The third line contains integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 2000</span>) — the number of elements in the array <span class="tex-font-style-tt">b</span>.</p><p>The fourth line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>b</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the elements of the array <span class="tex-font-style-tt">b</span>.</p>

## Output

<p>In the first line print the minimal value <span class="tex-span"><i>v</i> = |<i>s</i><sub class="lower-index"><i>a</i></sub> - <i>s</i><sub class="lower-index"><i>b</i></sub>|</span> that can be got with no more than two swaps.</p><p>The second line should contain the number of swaps <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 2</span>).</p><p>Each of the next <span class="tex-span"><i>k</i></span> lines should contain two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>p</i></sub>, <i>y</i><sub class="lower-index"><i>p</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>p</i></sub> ≤ <i>n</i>, 1 ≤ <i>y</i><sub class="lower-index"><i>p</i></sub> ≤ <i>m</i></span>) — the index of the element in the array <span class="tex-font-style-tt">a</span> and the index of the element in the array <span class="tex-font-style-tt">b</span> in the <span class="tex-span"><i>p</i></span>-th swap.</p><p>If there are several optimal solutions print any of them. Print the swaps in order the professor did them.</p>





```input1
5
5 4 3 2 1
4
1 1 1 1

```




```input2
5
1 2 3 4 5
1
15

```




```input3
5
1 2 3 4 5
4
1 2 3 4

```




```output1
1
2
1 1
4 2

```




```output2
0
0

```




```output3
1
1
3 1

```


