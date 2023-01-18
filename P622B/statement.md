## Description

<div><p>You are given the current time in <span class="tex-span">24</span>-hour format <span class="tex-font-style-tt">hh:mm</span>. Find and print the time after <span class="tex-span"><i>a</i></span> minutes.</p><p>Note that you should find only the time after <span class="tex-span"><i>a</i></span> minutes, see the examples to clarify the problem statement.</p><p>You can read more about <span class="tex-span">24</span>-hour format here <a href="https://en.wikipedia.org/wiki/24-hour_clock">https://en.wikipedia.org/wiki/24-hour_clock</a>.</p></div><div class="input-specification"><p>The first line contains the current time in the format <span class="tex-font-style-tt">hh:mm</span> (<span class="tex-span">0 ≤ <i>hh</i> &lt; 24, 0 ≤ <i>mm</i> &lt; 60</span>). The hours and the minutes are given with two digits (the hours or the minutes less than <span class="tex-span">10</span> are given with the leading zeroes).</p><p>The second line contains integer <span class="tex-span"><i>a</i></span> (<span class="tex-span">0 ≤ <i>a</i> ≤ 10<sup class="upper-index">4</sup></span>) — the number of the minutes passed.</p></div><div class="output-specification"><p>The only line should contain the time after <span class="tex-span"><i>a</i></span> minutes in the format described in the input. Note that you should print exactly two digits for the hours and the minutes (add leading zeroes to the numbers if needed).</p><p>See the examples to check the input/output format.</p></div>

## Input

<p>The first line contains the current time in the format <span class="tex-font-style-tt">hh:mm</span> (<span class="tex-span">0 ≤ <i>hh</i> &lt; 24, 0 ≤ <i>mm</i> &lt; 60</span>). The hours and the minutes are given with two digits (the hours or the minutes less than <span class="tex-span">10</span> are given with the leading zeroes).</p><p>The second line contains integer <span class="tex-span"><i>a</i></span> (<span class="tex-span">0 ≤ <i>a</i> ≤ 10<sup class="upper-index">4</sup></span>) — the number of the minutes passed.</p>

## Output

<p>The only line should contain the time after <span class="tex-span"><i>a</i></span> minutes in the format described in the input. Note that you should print exactly two digits for the hours and the minutes (add leading zeroes to the numbers if needed).</p><p>See the examples to check the input/output format.</p>





```input1
23:59
10

```




```input2
20:20
121

```




```input3
10:10
0

```




```output1
00:09

```




```output2
22:21

```




```output3
10:10

```


