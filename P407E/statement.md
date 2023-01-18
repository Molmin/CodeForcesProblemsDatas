## Description

<div><p>We'll call a sequence of integers a good <span class="tex-span"><i>k</i></span>-<span class="tex-span"><i>d</i></span> sequence if we can add to it at most <span class="tex-span"><i>k</i></span> numbers in such a way that after the sorting the sequence will be an arithmetic progression with difference <span class="tex-span"><i>d</i></span>.</p><p>You got hold of some sequence <span class="tex-span"><i>a</i></span>, consisting of <span class="tex-span"><i>n</i></span> integers. Your task is to find its longest contiguous subsegment, such that it is a good <span class="tex-span"><i>k</i></span>-<span class="tex-span"><i>d</i></span> sequence.</p></div><div class="input-specification"><p>The first line contains three space-separated integers <span class="tex-span"><i>n</i>, <i>k</i>, <i>d</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup>;&nbsp;0 ≤ <i>k</i> ≤ 2·10<sup class="upper-index">5</sup>;&nbsp;0 ≤ <i>d</i> ≤ 10<sup class="upper-index">9</sup></span>). The second line contains <span class="tex-span"><i>n</i></span> space-separated integers: <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the actual sequence.</p></div><div class="output-specification"><p>Print two space-separated integers <span class="tex-span"><i>l</i>, <i>r</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>) show that sequence <span class="tex-span"><i>a</i><sub class="lower-index"><i>l</i></sub>, <i>a</i><sub class="lower-index"><i>l</i> + 1</sub>, ..., <i>a</i><sub class="lower-index"><i>r</i></sub></span> is the longest subsegment that is a good <span class="tex-span"><i>k</i></span>-<span class="tex-span"><i>d</i></span> sequence.</p><p>If there are multiple optimal answers, print the one with the minimum value of <span class="tex-span"><i>l</i></span>.</p></div>

## Input

<p>The first line contains three space-separated integers <span class="tex-span"><i>n</i>, <i>k</i>, <i>d</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup>;&nbsp;0 ≤ <i>k</i> ≤ 2·10<sup class="upper-index">5</sup>;&nbsp;0 ≤ <i>d</i> ≤ 10<sup class="upper-index">9</sup></span>). The second line contains <span class="tex-span"><i>n</i></span> space-separated integers: <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the actual sequence.</p>

## Output

<p>Print two space-separated integers <span class="tex-span"><i>l</i>, <i>r</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>) show that sequence <span class="tex-span"><i>a</i><sub class="lower-index"><i>l</i></sub>, <i>a</i><sub class="lower-index"><i>l</i> + 1</sub>, ..., <i>a</i><sub class="lower-index"><i>r</i></sub></span> is the longest subsegment that is a good <span class="tex-span"><i>k</i></span>-<span class="tex-span"><i>d</i></span> sequence.</p><p>If there are multiple optimal answers, print the one with the minimum value of <span class="tex-span"><i>l</i></span>.</p>





```input1
6 1 2
4 3 2 8 6 2

```




```output1
3 5

```



## Note

<p>In the first test sample the answer is the subsegment consisting of numbers 2, 8, 6&nbsp;— after adding number 4 and sorting it becomes sequence 2, 4, 6, 8&nbsp;— the arithmetic progression with difference 2.</p>
