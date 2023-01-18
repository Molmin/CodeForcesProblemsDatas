## Description

<div><p><span class="tex-font-style-it">Even if the world is full of counterfeits, I still regard it as wonderful.</span></p><p>Pile up herbs and incense, and arise again from the flames and ashes of its predecessor&nbsp;— as is known to many, the phoenix does it like this.</p><p>The phoenix has a rather long lifespan, and reincarnates itself once every <span class="tex-span"><i>a</i>!</span> years. Here <span class="tex-span"><i>a</i>!</span> denotes the factorial of integer <span class="tex-span"><i>a</i></span>, that is, <span class="tex-span"><i>a</i>! = 1 × 2 × ... × <i>a</i></span>. Specifically, <span class="tex-span">0! = 1</span>.</p><p>Koyomi doesn't care much about this, but before he gets into another mess with oddities, he is interested in the number of times the phoenix will reincarnate in a timespan of <span class="tex-span"><i>b</i>!</span> years, that is, <img align="middle" class="tex-formula" src="file://if8VdojV.png" style="max-width: 100.0%;max-height: 100.0%;">. Note that when <span class="tex-span"><i>b</i> ≥ <i>a</i></span> this value is always integer.</p><p>As the answer can be quite large, it would be enough for Koyomi just to know <span class="tex-font-style-bf">the last digit of the answer in decimal representation</span>. And you're here to provide Koyomi with this knowledge.</p></div><div class="input-specification"><p>The first and only line of input contains two space-separated integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">0 ≤ <i>a</i> ≤ <i>b</i> ≤ 10<sup class="upper-index">18</sup></span>).</p></div><div class="output-specification"><p>Output one line containing a single decimal digit&nbsp;— the last digit of the value that interests Koyomi.</p></div>

## Input

<p>The first and only line of input contains two space-separated integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">0 ≤ <i>a</i> ≤ <i>b</i> ≤ 10<sup class="upper-index">18</sup></span>).</p>

## Output

<p>Output one line containing a single decimal digit&nbsp;— the last digit of the value that interests Koyomi.</p>





```input1
2 4

```




```input2
0 10

```




```input3
107 109

```




```output1
2

```




```output2
0

```




```output3
2

```



## Note

<p>In the first example, the last digit of <img align="middle" class="tex-formula" src="file://gpoXiWwb.png" style="max-width: 100.0%;max-height: 100.0%;"> is <span class="tex-span">2</span>;</p><p>In the second example, the last digit of <img align="middle" class="tex-formula" src="file://SY5YIAVn.png" style="max-width: 100.0%;max-height: 100.0%;"> is <span class="tex-span">0</span>;</p><p>In the third example, the last digit of <img align="middle" class="tex-formula" src="file://ce6g6wU9.png" style="max-width: 100.0%;max-height: 100.0%;"> is <span class="tex-span">2</span>.</p>
