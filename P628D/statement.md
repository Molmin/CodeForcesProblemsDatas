## Description

<div><p>Consider the decimal presentation of an integer. Let's call a number <span class="tex-font-style-tt">d-magic</span> if digit <span class="tex-span"><i>d</i></span> appears in decimal presentation of the number on even positions and nowhere else.</p><p>For example, the numbers <span class="tex-span">1727374</span>, <span class="tex-span">17</span>, <span class="tex-span">1</span> are <span class="tex-font-style-tt">7-magic</span> but <span class="tex-span">77</span>, <span class="tex-span">7</span>, <span class="tex-span">123</span>, <span class="tex-span">34</span>, <span class="tex-span">71</span> are not <span class="tex-font-style-tt">7-magic</span>. On the other hand the number <span class="tex-span">7</span> is <span class="tex-font-style-tt">0-magic</span>, <span class="tex-span">123</span> is <span class="tex-font-style-tt">2-magic</span>, <span class="tex-span">34</span> is <span class="tex-font-style-tt">4-magic</span> and <span class="tex-span">71</span> is <span class="tex-font-style-tt">1-magic</span>.</p><p>Find the number of <span class="tex-font-style-tt">d-magic</span> numbers in the segment <span class="tex-span">[<i>a</i>, <i>b</i>]</span> that are multiple of <span class="tex-span"><i>m</i></span>. Because the answer can be very huge you should only find its value modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span> (so you should find the remainder after dividing by <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>m</i>, <i>d</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 2000</span>, <span class="tex-span">0 ≤ <i>d</i> ≤ 9</span>) — the parameters from the problem statement.</p><p>The second line contains positive integer <span class="tex-span"><i>a</i></span> in decimal presentation (without leading zeroes).</p><p>The third line contains positive integer <span class="tex-span"><i>b</i></span> in decimal presentation (without leading zeroes).</p><p>It is guaranteed that <span class="tex-span"><i>a</i> ≤ <i>b</i></span>, the number of digits in <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> are the same and don't exceed <span class="tex-span">2000</span>.</p></div><div class="output-specification"><p>Print the only integer <span class="tex-span"><i>a</i></span> — the remainder after dividing by <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span> of the number of <span class="tex-font-style-tt">d-magic</span> numbers in segment <span class="tex-span">[<i>a</i>, <i>b</i>]</span> that are multiple of <span class="tex-span"><i>m</i></span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>m</i>, <i>d</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 2000</span>, <span class="tex-span">0 ≤ <i>d</i> ≤ 9</span>) — the parameters from the problem statement.</p><p>The second line contains positive integer <span class="tex-span"><i>a</i></span> in decimal presentation (without leading zeroes).</p><p>The third line contains positive integer <span class="tex-span"><i>b</i></span> in decimal presentation (without leading zeroes).</p><p>It is guaranteed that <span class="tex-span"><i>a</i> ≤ <i>b</i></span>, the number of digits in <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> are the same and don't exceed <span class="tex-span">2000</span>.</p>

## Output

<p>Print the only integer <span class="tex-span"><i>a</i></span> — the remainder after dividing by <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span> of the number of <span class="tex-font-style-tt">d-magic</span> numbers in segment <span class="tex-span">[<i>a</i>, <i>b</i>]</span> that are multiple of <span class="tex-span"><i>m</i></span>.</p>





```input1
2 6
10
99

```




```input2
2 0
1
9

```




```input3
19 7
1000
9999

```




```output1
8

```




```output2
4

```




```output3
6

```



## Note

<p>The numbers from the answer of the first example are <span class="tex-span">16</span>, <span class="tex-span">26</span>, <span class="tex-span">36</span>, <span class="tex-span">46</span>, <span class="tex-span">56</span>, <span class="tex-span">76</span>, <span class="tex-span">86</span> and <span class="tex-span">96</span>.</p><p>The numbers from the answer of the second example are <span class="tex-span">2</span>, <span class="tex-span">4</span>, <span class="tex-span">6</span> and <span class="tex-span">8</span>.</p><p>The numbers from the answer of the third example are <span class="tex-span">1767</span>, <span class="tex-span">2717</span>, <span class="tex-span">5757</span>, <span class="tex-span">6707</span>, <span class="tex-span">8797</span> and <span class="tex-span">9747</span>.</p>
