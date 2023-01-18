## Description

<div><p>Little Robber Girl likes to scare animals in her zoo for fun. She decided to arrange the animals in a row in the order of non-decreasing height. However, the animals were so scared that they couldn't stay in the right places.</p><p>The robber girl was angry at first, but then she decided to arrange the animals herself. She repeatedly names numbers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> such that <span class="tex-span"><i>r</i> - <i>l</i> + 1</span> is even. After that animals that occupy positions between <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> inclusively are rearranged as follows: the animal at position <span class="tex-span"><i>l</i></span> swaps places with the animal at position <span class="tex-span"><i>l</i> + 1</span>, the animal <span class="tex-span"><i>l</i> + 2</span> swaps with the animal <span class="tex-span"><i>l</i> + 3</span>, ..., finally, the animal at position <span class="tex-span"><i>r</i> - 1</span> swaps with the animal <span class="tex-span"><i>r</i></span>.</p><p>Help the robber girl to arrange the animals in the order of non-decreasing height. You should name at most <span class="tex-span">20 000</span> segments, since otherwise the robber girl will become bored and will start scaring the animals again.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>)&nbsp;— number of animals in the robber girl's zoo.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the height of the animal occupying the <span class="tex-span"><i>i</i></span>-th place.</p></div><div class="output-specification"><p>Print the sequence of operations that will rearrange the animals by non-decreasing height.</p><p>The output should contain several lines, <span class="tex-span"><i>i</i></span>-th of the lines should contain two space-separated integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> &lt; <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— descriptions of segments the robber girl should name. The segments should be described in the order the operations are performed.</p><p>The number of operations should not exceed <span class="tex-span">20 000</span>.</p><p>If the animals are arranged correctly from the start, you are allowed to output nothing.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>)&nbsp;— number of animals in the robber girl's zoo.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the height of the animal occupying the <span class="tex-span"><i>i</i></span>-th place.</p>

## Output

<p>Print the sequence of operations that will rearrange the animals by non-decreasing height.</p><p>The output should contain several lines, <span class="tex-span"><i>i</i></span>-th of the lines should contain two space-separated integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> &lt; <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— descriptions of segments the robber girl should name. The segments should be described in the order the operations are performed.</p><p>The number of operations should not exceed <span class="tex-span">20 000</span>.</p><p>If the animals are arranged correctly from the start, you are allowed to output nothing.</p>





```input1
4
2 1 4 3

```




```input2
7
36 28 57 39 66 69 68

```




```input3
5
1 2 1 2 1

```




```output1
1 4

```




```output2
1 4
6 7

```




```output3
2 5
3 4
1 4
1 4

```



## Note

<p>Note that you don't have to minimize the number of operations. Any solution that performs at most <span class="tex-span">20 000</span> operations is allowed.</p>
