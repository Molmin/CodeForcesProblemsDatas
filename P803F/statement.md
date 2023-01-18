## Description

<div><p>Let's call a non-empty sequence of positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>... <i>a</i><sub class="lower-index"><i>k</i></sub></span> <span class="tex-font-style-it">coprime</span> if the greatest common divisor of all elements of this sequence is equal to <span class="tex-span">1</span>.</p><p>Given an array <span class="tex-span"><i>a</i></span> consisting of <span class="tex-span"><i>n</i></span> positive integers, find the number of its <span class="tex-font-style-it">coprime</span> subsequences. Since the answer may be very large, print it modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p><p>Note that two subsequences are considered different if chosen indices are different. For example, in the array <span class="tex-span">[1, 1]</span> there are <span class="tex-span">3</span> different subsequences: <span class="tex-span">[1]</span>, <span class="tex-span">[1]</span> and <span class="tex-span">[1, 1]</span>.</p></div><div class="input-specification"><p>The first line contains one integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100000</span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>... <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100000</span>).</p></div><div class="output-specification"><p>Print the number of <span class="tex-font-style-it">coprime</span> subsequences of <span class="tex-span"><i>a</i></span> modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first line contains one integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100000</span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>... <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100000</span>).</p>

## Output

<p>Print the number of <span class="tex-font-style-it">coprime</span> subsequences of <span class="tex-span"><i>a</i></span> modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
3
1 2 3

```




```input2
4
1 1 1 1

```




```input3
7
1 3 5 15 3 105 35

```




```output1
5

```




```output2
15

```




```output3
100

```



## Note

<p>In the first example <span class="tex-font-style-it">coprime</span> subsequences are: </p><ol> <li> <span class="tex-span">1</span> </li><li> <span class="tex-span">1, 2</span> </li><li> <span class="tex-span">1, 3</span> </li><li> <span class="tex-span">1, 2, 3</span> </li><li> <span class="tex-span">2, 3</span> </li></ol><p>In the second example all subsequences are <span class="tex-font-style-it">coprime</span>.</p>
