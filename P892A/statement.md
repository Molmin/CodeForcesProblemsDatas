## Description

<div><p>Jafar has <span class="tex-span"><i>n</i></span> cans of cola. Each can is described by two integers: remaining volume of cola <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and can's capacity <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"> ≤ </span> <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>).</p><p>Jafar has decided to pour all remaining cola into just <span class="tex-span">2</span> cans, determine if he can do this or not!</p></div><div class="input-specification"><p>The first line of the input contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— number of cola cans.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — volume of remaining cola in cans.</p><p>The third line contains <span class="tex-span"><i>n</i></span> space-separated integers that <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — capacities of the cans.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">YES</span>" (without quotes) if it is possible to pour all remaining cola in <span class="tex-span">2</span> cans. Otherwise print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p><p>You can print each letter in any case (upper or lower).</p></div>

## Input

<p>The first line of the input contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— number of cola cans.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — volume of remaining cola in cans.</p><p>The third line contains <span class="tex-span"><i>n</i></span> space-separated integers that <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — capacities of the cans.</p>

## Output

<p>Print "<span class="tex-font-style-tt">YES</span>" (without quotes) if it is possible to pour all remaining cola in <span class="tex-span">2</span> cans. Otherwise print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p><p>You can print each letter in any case (upper or lower).</p>





```input1
2
3 5
3 6

```




```input2
3
6 8 9
6 10 12

```




```input3
5
0 0 5 0 0
1 1 8 10 5

```




```input4
4
4 1 0 3
5 2 2 3

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




```output4
YES

```



## Note

<p>In the first sample, there are already <span class="tex-span">2</span> cans, so the answer is "<span class="tex-font-style-tt">YES</span>".</p>
