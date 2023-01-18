## Description

<div><p>Two integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> are <span class="tex-font-style-underline">compatible</span>, if the result of their bitwise "AND" equals zero, that is, <span class="tex-span"><i>a</i></span> <span class="tex-span">&amp;</span> <span class="tex-span"><i>b</i> = 0</span>. For example, numbers <span class="tex-span">90</span> <span class="tex-span">(1011010<sub class="lower-index">2</sub>)</span> and <span class="tex-span">36</span> <span class="tex-span">(100100<sub class="lower-index">2</sub>)</span> are compatible, as <span class="tex-span">1011010<sub class="lower-index">2</sub></span> <span class="tex-span">&amp;</span> <span class="tex-span">100100<sub class="lower-index">2</sub> = 0<sub class="lower-index">2</sub></span>, and numbers <span class="tex-span">3</span> <span class="tex-span">(11<sub class="lower-index">2</sub>)</span> and <span class="tex-span">6</span> <span class="tex-span">(110<sub class="lower-index">2</sub>)</span> are not compatible, as <span class="tex-span">11<sub class="lower-index">2</sub></span> <span class="tex-span">&amp;</span> <span class="tex-span">110<sub class="lower-index">2</sub> = 10<sub class="lower-index">2</sub></span>.</p><p>You are given an array of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. Your task is to find the following for each array element: is this element compatible with some other element from the given array? If the answer to this question is positive, then you also should find any suitable element.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>) — the number of elements in the given array. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 4·10<sup class="upper-index">6</sup></span>) — the elements of the given array. The numbers in the array can coincide.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>ans</i><sub class="lower-index"><i>i</i></sub></span>. If <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> isn't compatible with any other element of the given array <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>, then <span class="tex-span"><i>ans</i><sub class="lower-index"><i>i</i></sub></span> should be equal to -1. Otherwise <span class="tex-span"><i>ans</i><sub class="lower-index"><i>i</i></sub></span> is any such number, that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">&amp;</span> <span class="tex-span"><i>ans</i><sub class="lower-index"><i>i</i></sub> = 0</span>, and also <span class="tex-span"><i>ans</i><sub class="lower-index"><i>i</i></sub></span> occurs in the array <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>) — the number of elements in the given array. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 4·10<sup class="upper-index">6</sup></span>) — the elements of the given array. The numbers in the array can coincide.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>ans</i><sub class="lower-index"><i>i</i></sub></span>. If <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> isn't compatible with any other element of the given array <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>, then <span class="tex-span"><i>ans</i><sub class="lower-index"><i>i</i></sub></span> should be equal to -1. Otherwise <span class="tex-span"><i>ans</i><sub class="lower-index"><i>i</i></sub></span> is any such number, that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">&amp;</span> <span class="tex-span"><i>ans</i><sub class="lower-index"><i>i</i></sub> = 0</span>, and also <span class="tex-span"><i>ans</i><sub class="lower-index"><i>i</i></sub></span> occurs in the array <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>.</p>





```input1
2
90 36

```




```input2
4
3 6 3 6

```




```input3
5
10 6 9 8 2

```




```output1
36 90
```




```output2
-1 -1 -1 -1
```




```output3
-1 8 2 2 8
```


