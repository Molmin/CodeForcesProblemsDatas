## Description

<div><p><span class="tex-font-style-it">Unlucky</span> year in Berland is such a year that its number <span class="tex-span"><i>n</i></span> can be represented as <span class="tex-span"><i>n</i> = <i>x</i><sup class="upper-index"><i>a</i></sup> + <i>y</i><sup class="upper-index"><i>b</i></sup></span>, where <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> are non-negative integer numbers. </p><p>For example, if <span class="tex-span"><i>x</i> = 2</span> and <span class="tex-span"><i>y</i> = 3</span> then the years <span class="tex-font-style-tt">4</span> and <span class="tex-font-style-tt">17</span> are <span class="tex-font-style-it">unlucky</span> (<span class="tex-span">4 = 2<sup class="upper-index">0</sup> + 3<sup class="upper-index">1</sup></span>, <span class="tex-span">17 = 2<sup class="upper-index">3</sup> + 3<sup class="upper-index">2</sup> = 2<sup class="upper-index">4</sup> + 3<sup class="upper-index">0</sup></span>) and year <span class="tex-font-style-tt">18</span> isn't <span class="tex-font-style-it">unlucky</span> as there is no such representation for it.</p><p>Such interval of years that there are no <span class="tex-font-style-it">unlucky</span> years in it is called <span class="tex-font-style-it">The Golden Age</span>.</p><p>You should write a program which will find maximum length of <span class="tex-font-style-it">The Golden Age</span> which starts no earlier than the year <span class="tex-span"><i>l</i></span> and ends no later than the year <span class="tex-span"><i>r</i></span>. If all years in the interval <span class="tex-span">[<i>l</i>, <i>r</i>]</span> are <span class="tex-font-style-it">unlucky</span> then the answer is <span class="tex-font-style-tt">0</span>.</p></div><div class="input-specification"><p>The first line contains four integer numbers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span>, <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">2 ≤ <i>x</i>, <i>y</i> ≤ 10<sup class="upper-index">18</sup></span>, <span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ 10<sup class="upper-index">18</sup></span>).</p></div><div class="output-specification"><p>Print the maximum length of <span class="tex-font-style-it">The Golden Age</span> within the interval <span class="tex-span">[<i>l</i>, <i>r</i>]</span>.</p><p>If all years in the interval <span class="tex-span">[<i>l</i>, <i>r</i>]</span> are <span class="tex-font-style-it">unlucky</span> then print <span class="tex-font-style-tt">0</span>.</p></div>

## Input

<p>The first line contains four integer numbers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span>, <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">2 ≤ <i>x</i>, <i>y</i> ≤ 10<sup class="upper-index">18</sup></span>, <span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ 10<sup class="upper-index">18</sup></span>).</p>

## Output

<p>Print the maximum length of <span class="tex-font-style-it">The Golden Age</span> within the interval <span class="tex-span">[<i>l</i>, <i>r</i>]</span>.</p><p>If all years in the interval <span class="tex-span">[<i>l</i>, <i>r</i>]</span> are <span class="tex-font-style-it">unlucky</span> then print <span class="tex-font-style-tt">0</span>.</p>





```input1
2 3 1 10

```




```input2
3 5 10 22

```




```input3
2 3 3 5

```




```output1
1

```




```output2
8

```




```output3
0

```



## Note

<p>In the first example the <span class="tex-font-style-it">unlucky</span> years are <span class="tex-font-style-tt">2, 3, 4, 5, 7, 9</span> and <span class="tex-font-style-tt">10</span>. So maximum length of <span class="tex-font-style-it">The Golden Age</span> is achived in the intervals <span class="tex-span">[1, 1]</span>, <span class="tex-span">[6, 6]</span> and <span class="tex-span">[8, 8]</span>.</p><p>In the second example the longest <span class="tex-font-style-it">Golden Age</span> is the interval <span class="tex-span">[15, 22]</span>.</p>
