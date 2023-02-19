## Description

<div><p>For given <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> find the number of distinct geometrical progression, each of which contains <span class="tex-span"><i>n</i></span> distinct integers not less than <span class="tex-span"><i>l</i></span> and not greater than <span class="tex-span"><i>r</i></span>. In other words, for each progression the following must hold: <span class="tex-span"><i>l</i> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>a</i><sub class="lower-index"><i>j</i></sub></span> , where <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> is the geometrical progression, <span class="tex-span">1 ≤ <i>i</i>, <i>j</i> ≤ <i>n</i></span> and <span class="tex-span"><i>i</i> ≠ <i>j</i></span>.</p><p>Geometrical progression is a sequence of numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> where each term after first is found by multiplying the previous one by a fixed non-zero number <span class="tex-span"><i>d</i></span> called the common ratio. Note that in our task <span class="tex-span"><i>d</i></span> may be non-integer. For example in progression <span class="tex-span">4, 6, 9</span>, common ratio is <img align="middle" class="tex-formula" src="file://9YK8bYHa.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>Two progressions <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> are considered different, if there is such <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>.</p></div><div class="input-specification"><p>The first and the only line cotains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">7</sup>, 1 ≤ <i>l</i> ≤ <i>r</i> ≤ 10<sup class="upper-index">7</sup></span>).</p></div><div class="output-specification"><p>Print the integer <span class="tex-span"><i>K</i></span>&nbsp;— is the answer to the problem.</p></div>

## Input

<p>The first and the only line cotains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">7</sup>, 1 ≤ <i>l</i> ≤ <i>r</i> ≤ 10<sup class="upper-index">7</sup></span>).</p>

## Output

<p>Print the integer <span class="tex-span"><i>K</i></span>&nbsp;— is the answer to the problem.</p>





```input1
1 1 10

```




```input2
2 6 9

```




```input3
3 1 10

```




```input4
3 3 10

```




```output1
10
```




```output2
12
```




```output3
8
```




```output4
2
```



## Note

<p>These are possible progressions for the first test of examples: </p><ul> <li> <span class="tex-span">1</span>; </li><li> <span class="tex-span">2</span>; </li><li> <span class="tex-span">3</span>; </li><li> <span class="tex-span">4</span>; </li><li> <span class="tex-span">5</span>; </li><li> <span class="tex-span">6</span>; </li><li> <span class="tex-span">7</span>; </li><li> <span class="tex-span">8</span>; </li><li> <span class="tex-span">9</span>; </li><li> <span class="tex-span">10</span>. </li></ul><p>These are possible progressions for the second test of examples: </p><ul> <li> <span class="tex-span">6, 7</span>; </li><li> <span class="tex-span">6, 8</span>; </li><li> <span class="tex-span">6, 9</span>; </li><li> <span class="tex-span">7, 6</span>; </li><li> <span class="tex-span">7, 8</span>; </li><li> <span class="tex-span">7, 9</span>; </li><li> <span class="tex-span">8, 6</span>; </li><li> <span class="tex-span">8, 7</span>; </li><li> <span class="tex-span">8, 9</span>; </li><li> <span class="tex-span">9, 6</span>; </li><li> <span class="tex-span">9, 7</span>; </li><li> <span class="tex-span">9, 8</span>. </li></ul><p>These are possible progressions for the third test of examples: </p><ul> <li> <span class="tex-span">1, 2, 4</span>; </li><li> <span class="tex-span">1, 3, 9</span>; </li><li> <span class="tex-span">2, 4, 8</span>; </li><li> <span class="tex-span">4, 2, 1</span>; </li><li> <span class="tex-span">4, 6, 9</span>; </li><li> <span class="tex-span">8, 4, 2</span>; </li><li> <span class="tex-span">9, 3, 1</span>; </li><li> <span class="tex-span">9, 6, 4</span>. </li></ul><p>These are possible progressions for the fourth test of examples: </p><ul> <li> <span class="tex-span">4, 6, 9</span>; </li><li> <span class="tex-span">9, 6, 4</span>. </li></ul>
