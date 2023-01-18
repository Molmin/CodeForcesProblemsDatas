## Description

<div><p>You have an array <span class="tex-span"><i>a</i></span> with length <span class="tex-span"><i>n</i></span>, you can perform operations. Each operation is like this: choose two <span class="tex-font-style-bf">adjacent</span> elements from <span class="tex-span"><i>a</i></span>, say <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>, and replace one of them with <span class="tex-span"><i>gcd</i>(<i>x</i>, <i>y</i>)</span>, where <span class="tex-span"><i>gcd</i></span> denotes the <a href="https://en.wikipedia.org/wiki/Greatest_common_divisor">greatest common divisor</a>.</p><p>What is the minimum number of operations you need to make all of the elements equal to <span class="tex-span">1</span>?</p></div><div class="input-specification"><p>The first line of the input contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2000</span>) — the number of elements in the array.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the elements of the array.</p></div><div class="output-specification"><p>Print <span class="tex-font-style-tt">-1</span>, if it is impossible to turn all numbers to <span class="tex-span">1</span>. Otherwise, print the minimum number of operations needed to make all numbers equal to <span class="tex-span">1</span>.</p></div>

## Input

<p>The first line of the input contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2000</span>) — the number of elements in the array.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the elements of the array.</p>

## Output

<p>Print <span class="tex-font-style-tt">-1</span>, if it is impossible to turn all numbers to <span class="tex-span">1</span>. Otherwise, print the minimum number of operations needed to make all numbers equal to <span class="tex-span">1</span>.</p>





```input1
5
2 2 3 4 6

```




```input2
4
2 4 6 8

```




```input3
3
2 6 9

```




```output1
5

```




```output2
-1

```




```output3
4

```



## Note

<p>In the first sample you can turn all numbers to <span class="tex-span">1</span> using the following <span class="tex-span">5</span> moves:</p><ul> <li> <span class="tex-span">[2, 2, 3, 4, 6]</span>. </li><li> <span class="tex-span">[2, 1, 3, 4, 6]</span> </li><li> <span class="tex-span">[2, 1, 3, 1, 6]</span> </li><li> <span class="tex-span">[2, 1, 1, 1, 6]</span> </li><li> <span class="tex-span">[1, 1, 1, 1, 6]</span> </li><li> <span class="tex-span">[1, 1, 1, 1, 1]</span> </li></ul><p>We can prove that in this case it is not possible to make all numbers one using less than <span class="tex-span">5</span> moves.</p>
