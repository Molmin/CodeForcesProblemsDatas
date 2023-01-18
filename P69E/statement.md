## Description

<div><p>Programmer Sasha has recently begun to study data structures. His coach Stas told him to solve the problem of finding a minimum on the segment of the array in <img align="middle" class="tex-formula" src="file://PBZuWxmC.png" style="max-width: 100.0%;max-height: 100.0%;">, which Sasha coped with. For Sasha not to think that he had learned all, Stas gave him a new task. For each segment of the fixed length Sasha must find the maximum element of those that occur on the given segment exactly once. Help Sasha solve this problem. </p></div><div class="input-specification"><p>The first line contains two positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>k</i> ≤ <i>n</i></span>) — the number of array elements and the length of the segment. </p><p>Then follow <span class="tex-span"><i>n</i></span> lines: the <span class="tex-span"><i>i</i></span>-th one contains a single number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). </p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i>–<i>k</i> + 1</span> numbers, one per line: on the <span class="tex-span"><i>i</i></span>-th line print of the maximum number of those numbers from the subarray <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i> + 1</sub></span> … <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i> + <i>k</i> - 1</sub></span> that occur in this subarray exactly 1 time. If there are no such numbers in this subarray, print "<span class="tex-font-style-tt">Nothing</span>".</p></div>

## Input

<p>The first line contains two positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>k</i> ≤ <i>n</i></span>) — the number of array elements and the length of the segment. </p><p>Then follow <span class="tex-span"><i>n</i></span> lines: the <span class="tex-span"><i>i</i></span>-th one contains a single number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). </p>

## Output

<p>Print <span class="tex-span"><i>n</i>–<i>k</i> + 1</span> numbers, one per line: on the <span class="tex-span"><i>i</i></span>-th line print of the maximum number of those numbers from the subarray <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i> + 1</sub></span> … <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i> + <i>k</i> - 1</sub></span> that occur in this subarray exactly 1 time. If there are no such numbers in this subarray, print "<span class="tex-font-style-tt">Nothing</span>".</p>





```input1
5 3
1
2
2
3
3

```




```input2
6 4
3
3
3
4
4
2

```




```output1
1
3
2

```




```output2
4
Nothing
3

```


