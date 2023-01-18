## Description

<div><p>SmallR likes a game called "Deleting Substrings". In the game you are given a sequence of integers <span class="tex-span"><i>w</i></span>, you can modify the sequence and get points. The only type of modification you can perform is (unexpected, right?) deleting substrings. More formally, you can choose several contiguous elements of <span class="tex-span"><i>w</i></span> and delete them from the sequence. Let's denote the sequence of chosen elements as <span class="tex-span"><i>w</i><sub class="lower-index"><i>l</i></sub>, <i>w</i><sub class="lower-index"><i>l</i> + 1</sub>, ..., <i>w</i><sub class="lower-index"><i>r</i></sub></span>. They must meet the conditions:</p><ul> <li> the equality <span class="tex-span">|<i>w</i><sub class="lower-index"><i>i</i></sub> - <i>w</i><sub class="lower-index"><i>i</i> + 1</sub>| = 1</span> must hold for all <span class="tex-span"><i>i</i></span> <span class="tex-span">(<i>l</i> ≤ <i>i</i> &lt; <i>r</i>)</span>; </li><li> the inequality <span class="tex-span">2·<i>w</i><sub class="lower-index"><i>i</i></sub> - <i>w</i><sub class="lower-index"><i>i</i> + 1</sub> - <i>w</i><sub class="lower-index"><i>i</i> - 1</sub> ≥ 0</span> must hold for all <span class="tex-span"><i>i</i></span> <span class="tex-span">(<i>l</i> &lt; <i>i</i> &lt; <i>r</i>)</span>. </li></ul><p>After deleting the chosen substring of <span class="tex-span"><i>w</i></span>, you gain <span class="tex-span"><i>v</i><sub class="lower-index"><i>r</i> - <i>l</i> + 1</sub></span> points. You can perform the described operation again and again while proper substrings exist. Also you can end the game at any time. Your task is to calculate the maximum total score you can get in the game.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 400)</span> — the initial length of <span class="tex-span"><i>w</i></span>. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>v</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">2</sub>, ..., <i>v</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ |<i>v</i><sub class="lower-index"><i>i</i></sub>| ≤ 2000)</span> — the costs of operations. The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>w</i><sub class="lower-index">1</sub>, <i>w</i><sub class="lower-index">2</sub>, ..., <i>w</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> — the initial <span class="tex-span"><i>w</i></span>.</p></div><div class="output-specification"><p>Print a single integer — the maximum total score you can get.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 400)</span> — the initial length of <span class="tex-span"><i>w</i></span>. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>v</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">2</sub>, ..., <i>v</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ |<i>v</i><sub class="lower-index"><i>i</i></sub>| ≤ 2000)</span> — the costs of operations. The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>w</i><sub class="lower-index">1</sub>, <i>w</i><sub class="lower-index">2</sub>, ..., <i>w</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> — the initial <span class="tex-span"><i>w</i></span>.</p>

## Output

<p>Print a single integer — the maximum total score you can get.</p>





```input1
3
0 0 3
1 2 1

```




```input2
6
1 4 5 6 7 1000
2 1 1 2 2 3

```




```output1
3
```




```output2
12
```


