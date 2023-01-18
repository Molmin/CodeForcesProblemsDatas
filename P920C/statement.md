## Description

<div><p>You have an array <span class="tex-span"><i>a</i></span> consisting of <span class="tex-span"><i>n</i></span> integers. Each integer from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> appears exactly once in this array.</p><p>For some indices <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i> - 1</span>) it is possible to swap <span class="tex-span"><i>i</i></span>-th element with <span class="tex-span">(<i>i</i> + 1)</span>-th, for other indices it is not possible. You may perform any number of swapping operations any order. There is no limit on the number of times you swap <span class="tex-span"><i>i</i></span>-th element with <span class="tex-span">(<i>i</i> + 1)</span>-th (if the position is not forbidden).</p><p>Can you make this array sorted in ascending order performing some sequence of swapping operations?</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 200000</span>) — the number of elements in the array.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 200000</span>) — the elements of the array. Each integer from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> appears exactly once.</p><p>The third line contains a string of <span class="tex-span"><i>n</i> - 1</span> characters, each character is either <span class="tex-font-style-tt">0</span> or <span class="tex-font-style-tt">1</span>. If <span class="tex-span"><i>i</i></span>-th character is <span class="tex-font-style-tt">1</span>, then you can swap <span class="tex-span"><i>i</i></span>-th element with <span class="tex-span">(<i>i</i> + 1)</span>-th any number of times, otherwise it is forbidden to swap <span class="tex-span"><i>i</i></span>-th element with <span class="tex-span">(<i>i</i> + 1)</span>-th.</p></div><div class="output-specification"><p>If it is possible to sort the array in ascending order using any sequence of swaps you are allowed to make, print <span class="tex-font-style-tt">YES</span>. Otherwise, print <span class="tex-font-style-tt">NO</span>.</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 200000</span>) — the number of elements in the array.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 200000</span>) — the elements of the array. Each integer from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> appears exactly once.</p><p>The third line contains a string of <span class="tex-span"><i>n</i> - 1</span> characters, each character is either <span class="tex-font-style-tt">0</span> or <span class="tex-font-style-tt">1</span>. If <span class="tex-span"><i>i</i></span>-th character is <span class="tex-font-style-tt">1</span>, then you can swap <span class="tex-span"><i>i</i></span>-th element with <span class="tex-span">(<i>i</i> + 1)</span>-th any number of times, otherwise it is forbidden to swap <span class="tex-span"><i>i</i></span>-th element with <span class="tex-span">(<i>i</i> + 1)</span>-th.</p>

## Output

<p>If it is possible to sort the array in ascending order using any sequence of swaps you are allowed to make, print <span class="tex-font-style-tt">YES</span>. Otherwise, print <span class="tex-font-style-tt">NO</span>.</p>





```input1
6
1 2 5 3 4 6
01110

```




```input2
6
1 2 5 3 4 6
01010

```




```output1
YES

```




```output2
NO

```



## Note

<p>In the first example you may swap <span class="tex-span"><i>a</i><sub class="lower-index">3</sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index">4</sub></span>, and then swap <span class="tex-span"><i>a</i><sub class="lower-index">4</sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index">5</sub></span>.</p>
