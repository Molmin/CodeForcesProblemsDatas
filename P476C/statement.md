## Description

<div><p>Dreamoon loves summing up something for no reason. One day he obtains two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> occasionally. He wants to calculate the sum of all <span class="tex-font-style-it">nice</span> integers. Positive integer <span class="tex-span"><i>x</i></span> is called <span class="tex-font-style-it">nice</span> if <img align="middle" class="tex-formula" src="file://wtkVGROs.png" style="max-width: 100.0%;max-height: 100.0%;"> and <img align="middle" class="tex-formula" src="file://UpLrZkef.png" style="max-width: 100.0%;max-height: 100.0%;">, where <span class="tex-span"><i>k</i></span> is some <span class="tex-font-style-bf">integer</span> number in range <span class="tex-span">[1, <i>a</i>]</span>.</p><p>By <img align="middle" class="tex-formula" src="file://TjWt7NoH.png" style="max-width: 100.0%;max-height: 100.0%;"> we denote the <span class="tex-font-style-it">quotient</span> of integer division of <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>. By <img align="middle" class="tex-formula" src="file://oNngD1LJ.png" style="max-width: 100.0%;max-height: 100.0%;"> we denote the <span class="tex-font-style-it">remainder</span> of integer division of <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>. You can read more about these operations here: <span class="tex-font-style-tt">http://goo.gl/AcsXhT</span>.</p><p>The answer may be large, so please print its remainder modulo <span class="tex-span">1 000 000 007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>). Can you compute it faster than Dreamoon?</p></div><div class="input-specification"><p>The single line of the input contains two integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ 10<sup class="upper-index">7</sup></span>).</p></div><div class="output-specification"><p>Print a single integer representing the answer modulo <span class="tex-span">1 000 000 007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p></div>

## Input

<p>The single line of the input contains two integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ 10<sup class="upper-index">7</sup></span>).</p>

## Output

<p>Print a single integer representing the answer modulo <span class="tex-span">1 000 000 007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p>





```input1
1 1

```




```input2
2 2

```




```output1
0

```




```output2
8

```



## Note

<p>For the first sample, there are no nice integers because <img align="middle" class="tex-formula" src="file://eBXNbItf.png" style="max-width: 100.0%;max-height: 100.0%;"> is always zero.</p><p>For the second sample, the set of nice integers is <span class="tex-span">{3, 5}</span>.</p>
