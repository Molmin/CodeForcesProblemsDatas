## Description

<div><p>The array <span class="tex-span"><i>a</i></span> with <span class="tex-span"><i>n</i></span> integers is given. Let's call the sequence of one or more consecutive elements in <span class="tex-span"><i>a</i></span> <span class="tex-font-style-tt">segment</span>. Also let's call the segment <span class="tex-font-style-it">k</span>-<span class="tex-font-style-tt">good</span> if it contains no more than <span class="tex-span"><i>k</i></span> different values.</p><p>Find any longest <span class="tex-font-style-it">k</span>-good segment.</p><p>As the input/output can reach huge size it is recommended to use fast input/output methods: for example, prefer to use <span class="tex-font-style-tt">scanf/printf</span> instead of <span class="tex-font-style-tt">cin/cout</span> in C++, prefer to use <span class="tex-font-style-tt">BufferedReader/PrintWriter</span> instead of <span class="tex-font-style-tt">Scanner/System.out</span> in <span class="tex-font-style-tt">Java</span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i>, <i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup></span>) — the number of elements in <span class="tex-span"><i>a</i></span> and the parameter <span class="tex-span"><i>k</i></span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — the elements of the array <span class="tex-span"><i>a</i></span>.</p></div><div class="output-specification"><p>Print two integers <span class="tex-span"><i>l</i>, <i>r</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>) — the index of the left and the index of the right ends of some <span class="tex-font-style-it">k</span>-good longest segment. If there are several longest segments you can print any of them. The elements in <span class="tex-span"><i>a</i></span> are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from left to right.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i>, <i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup></span>) — the number of elements in <span class="tex-span"><i>a</i></span> and the parameter <span class="tex-span"><i>k</i></span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — the elements of the array <span class="tex-span"><i>a</i></span>.</p>

## Output

<p>Print two integers <span class="tex-span"><i>l</i>, <i>r</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>) — the index of the left and the index of the right ends of some <span class="tex-font-style-it">k</span>-good longest segment. If there are several longest segments you can print any of them. The elements in <span class="tex-span"><i>a</i></span> are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from left to right.</p>





```input1
5 5
1 2 3 4 5

```




```input2
9 3
6 5 1 2 3 2 1 4 5

```




```input3
3 1
1 2 3

```




```output1
1 5

```




```output2
3 7

```




```output3
1 1

```


