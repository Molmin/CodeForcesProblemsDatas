## Description

<div><p>After finishing eating her bun, Alyona came up with two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span>. She decided to write down two columns of integers&nbsp;— the first column containing integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> and the second containing integers from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>. Now the girl wants to count how many pairs of integers she can choose, one from the first column and the other from the second column, such that their sum is divisible by <span class="tex-span">5</span>.</p><p>Formally, Alyona wants to count the number of pairs of integers <span class="tex-span">(<i>x</i>, <i>y</i>)</span> such that <span class="tex-span">1 ≤ <i>x</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>y</i> ≤ <i>m</i></span> and <img align="middle" class="tex-formula" src="file://i1A2ePLn.png" style="max-width: 100.0%;max-height: 100.0%;"> equals <span class="tex-span">0</span>.</p><p>As usual, Alyona has some troubles and asks you to help.</p></div><div class="input-specification"><p>The only line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1 000 000</span>).</p></div><div class="output-specification"><p>Print the only integer&nbsp;— the number of pairs of integers <span class="tex-span">(<i>x</i>, <i>y</i>)</span> such that <span class="tex-span">1 ≤ <i>x</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>y</i> ≤ <i>m</i></span> and <span class="tex-span">(<i>x</i> + <i>y</i>)</span> is divisible by <span class="tex-span">5</span>.</p></div>

## Input

<p>The only line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1 000 000</span>).</p>

## Output

<p>Print the only integer&nbsp;— the number of pairs of integers <span class="tex-span">(<i>x</i>, <i>y</i>)</span> such that <span class="tex-span">1 ≤ <i>x</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>y</i> ≤ <i>m</i></span> and <span class="tex-span">(<i>x</i> + <i>y</i>)</span> is divisible by <span class="tex-span">5</span>.</p>





```input1
6 12

```




```input2
11 14

```




```input3
1 5

```




```input4
3 8

```




```input5
5 7

```




```input6
21 21

```




```output1
14

```




```output2
31

```




```output3
1

```




```output4
5

```




```output5
7

```




```output6
88

```



## Note

<p>Following pairs are suitable in the first sample case: </p><ul> <li> for <span class="tex-span"><i>x</i> = 1</span> fits <span class="tex-span"><i>y</i></span> equal to <span class="tex-span">4</span> or <span class="tex-span">9</span>; </li><li> for <span class="tex-span"><i>x</i> = 2</span> fits <span class="tex-span"><i>y</i></span> equal to <span class="tex-span">3</span> or <span class="tex-span">8</span>; </li><li> for <span class="tex-span"><i>x</i> = 3</span> fits <span class="tex-span"><i>y</i></span> equal to <span class="tex-span">2</span>, <span class="tex-span">7</span> or <span class="tex-span">12</span>; </li><li> for <span class="tex-span"><i>x</i> = 4</span> fits <span class="tex-span"><i>y</i></span> equal to <span class="tex-span">1</span>, <span class="tex-span">6</span> or <span class="tex-span">11</span>; </li><li> for <span class="tex-span"><i>x</i> = 5</span> fits <span class="tex-span"><i>y</i></span> equal to <span class="tex-span">5</span> or <span class="tex-span">10</span>; </li><li> for <span class="tex-span"><i>x</i> = 6</span> fits <span class="tex-span"><i>y</i></span> equal to <span class="tex-span">4</span> or <span class="tex-span">9</span>. </li></ul><p>Only the pair <span class="tex-span">(1, 4)</span> is suitable in the third sample case.</p>
