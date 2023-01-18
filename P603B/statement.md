## Description

<div><p>As behooves any intelligent schoolboy, Kevin Sun is studying psycowlogy, cowculus, and cryptcowgraphy at the Bovinia State University (BGU) under Farmer Ivan. During his Mathematics of Olympiads (MoO) class, Kevin was confronted with a weird functional equation and needs your help. For two fixed integers <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>p</i></span>, where <span class="tex-span"><i>p</i></span> is an odd prime number, the functional equation states that </p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://9OBdeXi8.png" style="max-width: 100.0%;max-height: 100.0%;"></center> <p>for some function <img align="middle" class="tex-formula" src="file://HEDYjWyh.png" style="max-width: 100.0%;max-height: 100.0%;">. (This equation should hold for any integer <span class="tex-span"><i>x</i></span> in the range <span class="tex-span">0</span> to <span class="tex-span"><i>p</i> - 1</span>, inclusive.)</p><p>It turns out that <span class="tex-span"><i>f</i></span> can actually be many different functions. Instead of finding a solution, Kevin wants you to count the number of distinct functions <span class="tex-span"><i>f</i></span> that satisfy this equation. Since the answer may be very large, you should print your result modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>The input consists of two space-separated integers <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">3 ≤ <i>p</i> ≤ 1 000 000</span>, <span class="tex-span">0 ≤ <i>k</i> ≤ <i>p</i> - 1</span>) on a single line. It is guaranteed that <span class="tex-span"><i>p</i></span> is an odd prime number.</p></div><div class="output-specification"><p>Print a single integer, the number of distinct functions <span class="tex-span"><i>f</i></span> modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The input consists of two space-separated integers <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">3 ≤ <i>p</i> ≤ 1 000 000</span>, <span class="tex-span">0 ≤ <i>k</i> ≤ <i>p</i> - 1</span>) on a single line. It is guaranteed that <span class="tex-span"><i>p</i></span> is an odd prime number.</p>

## Output

<p>Print a single integer, the number of distinct functions <span class="tex-span"><i>f</i></span> modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
3 2

```




```input2
5 4

```




```output1
3

```




```output2
25

```



## Note

<p>In the first sample, <span class="tex-span"><i>p</i> = 3</span> and <span class="tex-span"><i>k</i> = 2</span>. The following functions work: </p><ol> <li> <span class="tex-span"><i>f</i>(0) = 0</span>, <span class="tex-span"><i>f</i>(1) = 1</span>, <span class="tex-span"><i>f</i>(2) = 2</span>. </li><li> <span class="tex-span"><i>f</i>(0) = 0</span>, <span class="tex-span"><i>f</i>(1) = 2</span>, <span class="tex-span"><i>f</i>(2) = 1</span>. </li><li> <span class="tex-span"><i>f</i>(0) = <i>f</i>(1) = <i>f</i>(2) = 0</span>. </li></ol>
