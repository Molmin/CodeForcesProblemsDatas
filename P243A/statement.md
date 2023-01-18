## Description

<div><p>Polycarpus has a sequence, consisting of <span class="tex-span"><i>n</i></span> non-negative integers: <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>.</p><p>Let's define function <span class="tex-span"><i>f</i>(<i>l</i>, <i>r</i>)</span> (<span class="tex-span"><i>l</i>, <i>r</i></span> are integer, <span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>) for sequence <span class="tex-span"><i>a</i></span> as an operation of bitwise OR of all the sequence elements with indexes from <span class="tex-span"><i>l</i></span> to <span class="tex-span"><i>r</i></span>. Formally: <span class="tex-span"><i>f</i>(<i>l</i>, <i>r</i>) = <i>a</i><sub class="lower-index"><i>l</i></sub>&nbsp;|&nbsp;<i>a</i><sub class="lower-index"><i>l</i> + 1</sub>&nbsp;|&nbsp;... &nbsp;|&nbsp;<i>a</i><sub class="lower-index"><i>r</i></sub></span>. </p><p>Polycarpus took a piece of paper and wrote out the values of function <span class="tex-span"><i>f</i>(<i>l</i>, <i>r</i>)</span> for all <span class="tex-span"><i>l</i>, <i>r</i></span> (<span class="tex-span"><i>l</i>, <i>r</i></span> are integer, <span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>). Now he wants to know, how many <span class="tex-font-style-bf">distinct</span> values he's got in the end. </p><p>Help Polycarpus, count the number of distinct values of function <span class="tex-span"><i>f</i>(<i>l</i>, <i>r</i>)</span> for the given sequence <span class="tex-span"><i>a</i></span>.</p><p>Expression <span class="tex-span"><i>x</i>&nbsp;|&nbsp;<i>y</i></span> means applying the operation of bitwise OR to numbers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>. This operation exists in all modern programming languages, for example, in language <span class="tex-font-style-it">C++</span> and <span class="tex-font-style-it">Java</span> it is marked as "<span class="tex-font-style-tt">|</span>", in <span class="tex-font-style-it">Pascal</span> — as "<span class="tex-font-style-tt">or</span>".</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of elements of sequence <span class="tex-span"><i>a</i></span>. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup>)</span> — the elements of sequence <span class="tex-span"><i>a</i></span>.</p></div><div class="output-specification"><p>Print a single integer — the number of distinct values of function <span class="tex-span"><i>f</i>(<i>l</i>, <i>r</i>)</span> for the given sequence <span class="tex-span"><i>a</i></span>.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of elements of sequence <span class="tex-span"><i>a</i></span>. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup>)</span> — the elements of sequence <span class="tex-span"><i>a</i></span>.</p>

## Output

<p>Print a single integer — the number of distinct values of function <span class="tex-span"><i>f</i>(<i>l</i>, <i>r</i>)</span> for the given sequence <span class="tex-span"><i>a</i></span>.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
3
1 2 0

```




```input2
10
1 2 3 4 5 6 1 2 9 10

```




```output1
4
```




```output2
11
```



## Note

<p>In the first test case Polycarpus will have 6 numbers written on the paper: <span class="tex-span"><i>f</i>(1, 1) = 1</span>, <span class="tex-span"><i>f</i>(1, 2) = 3</span>, <span class="tex-span"><i>f</i>(1, 3) = 3</span>, <span class="tex-span"><i>f</i>(2, 2) = 2</span>, <span class="tex-span"><i>f</i>(2, 3) = 2</span>, <span class="tex-span"><i>f</i>(3, 3) = 0</span>. There are exactly <span class="tex-span">4</span> distinct numbers among them: <span class="tex-span">0, 1, 2, 3</span>.</p>
