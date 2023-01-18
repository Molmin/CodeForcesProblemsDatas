## Description

<div><p>It's now <span class="tex-span">260</span> AD. Shapur, being extremely smart, became the King of Persia. He is now called Shapur, His majesty King of kings of Iran and Aniran.</p><p>Recently the Romans declared war on Persia. They dreamed to occupy Armenia. In the recent war, the Romans were badly defeated. Now their senior army general, Philip is captured by Shapur and Shapur is now going to capture Valerian, the Roman emperor.</p><p>Being defeated, the cowardly Valerian hid in a room at the top of one of his castles. To capture him, Shapur has to open many doors. Fortunately Valerian was too scared to make impenetrable locks for the doors.</p><p>Each door has <span class="tex-span">4</span> parts. The first part is an integer number <span class="tex-span"><i>a</i></span>. The second part is either an integer number <span class="tex-span"><i>b</i></span> or some really odd sign which looks like <span class="tex-font-style-tt">R</span>. The third one is an integer <span class="tex-span"><i>c</i></span> and the fourth part is empty! As if it was laid for writing something. Being extremely gifted, after opening the first few doors, Shapur found out the secret behind the locks.</p><p><span class="tex-span"><i>c</i></span> is an integer written in base <span class="tex-span"><i>a</i></span>, to open the door we should write it in base <span class="tex-span"><i>b</i></span>. The only bad news is that this <span class="tex-font-style-tt">R</span> is some sort of special numbering system that is used only in Roman empire, so opening the doors is not just a piece of cake!</p><p>Here's an explanation of this really weird number system that even doesn't have zero:</p><p>Roman numerals are based on seven symbols: a stroke (identified with the letter <span class="tex-font-style-tt">I</span>) for a unit, a chevron (identified with the letter <span class="tex-font-style-tt">V</span>) for a five, a cross-stroke (identified with the letter <span class="tex-font-style-tt">X</span>) for a ten, a <span class="tex-font-style-tt">C</span> (identified as an abbreviation of Centum) for a hundred, etc.:</p><ul><li> <span class="tex-font-style-tt">I</span>=<span class="tex-span">1</span></li><li> <span class="tex-font-style-tt">V</span>=<span class="tex-span">5</span></li><li> <span class="tex-font-style-tt">X</span>=<span class="tex-span">10</span></li><li> <span class="tex-font-style-tt">L</span>=<span class="tex-span">50</span></li><li> <span class="tex-font-style-tt">C</span>=<span class="tex-span">100</span></li><li> <span class="tex-font-style-tt">D</span>=<span class="tex-span">500</span></li><li> <span class="tex-font-style-tt">M</span>=<span class="tex-span">1000</span></li></ul><p>Symbols are iterated to produce multiples of the decimal (<span class="tex-span">1</span>, <span class="tex-span">10</span>, <span class="tex-span">100</span>, <span class="tex-span">1, 000</span>) values, with <span class="tex-font-style-tt">V</span>, <span class="tex-font-style-tt">L</span>, <span class="tex-font-style-tt">D</span> substituted for a multiple of five, and the iteration continuing: <span class="tex-font-style-tt">I</span> <span class="tex-span">1</span>, <span class="tex-font-style-tt">II</span> <span class="tex-span">2</span>, <span class="tex-font-style-tt">III</span> <span class="tex-span">3</span>, <span class="tex-font-style-tt">V</span> <span class="tex-span">5</span>, <span class="tex-font-style-tt">VI</span> <span class="tex-span">6</span>, <span class="tex-font-style-tt">VII</span> <span class="tex-span">7</span>, etc., and the same for other bases: <span class="tex-font-style-tt">X</span> <span class="tex-span">10</span>, <span class="tex-font-style-tt">XX</span> <span class="tex-span">20</span>, <span class="tex-font-style-tt">XXX</span> <span class="tex-span">30</span>, <span class="tex-font-style-tt">L</span> <span class="tex-span">50</span>, <span class="tex-font-style-tt">LXXX</span> <span class="tex-span">80</span>; <span class="tex-font-style-tt">CC</span> <span class="tex-span">200</span>, <span class="tex-font-style-tt">DCC</span> <span class="tex-span">700</span>, etc. At the fourth and ninth iteration, a subtractive principle must be employed, with the base placed before the higher base: <span class="tex-font-style-tt">IV</span> <span class="tex-span">4</span>, <span class="tex-font-style-tt">IX</span> <span class="tex-span">9</span>, <span class="tex-font-style-tt">XL</span> <span class="tex-span">40</span>, <span class="tex-font-style-tt">XC</span> <span class="tex-span">90</span>, <span class="tex-font-style-tt">CD</span> <span class="tex-span">400</span>, <span class="tex-font-style-tt">CM</span> <span class="tex-span">900</span>.</p><p>Also in bases greater than <span class="tex-span">10</span> we use <span class="tex-font-style-tt">A</span> for <span class="tex-span">10</span>, <span class="tex-font-style-tt">B</span> for <span class="tex-span">11</span>, etc.</p><p>Help Shapur capture Valerian and bring peace back to Persia, especially Armenia.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">2 ≤ <i>a</i>, <i>b</i> ≤ 25</span>). Only <span class="tex-span"><i>b</i></span> may be replaced by an <span class="tex-font-style-tt">R</span> which indicates Roman numbering system.</p><p>The next line contains a single non-negative integer <span class="tex-span"><i>c</i></span> in base <span class="tex-span"><i>a</i></span> which may contain leading zeros but its length doesn't exceed <span class="tex-span">10<sup class="upper-index">3</sup></span>. </p><p>It is guaranteed that if we have Roman numerals included the number would be less than or equal to <span class="tex-span">3000<sub class="lower-index">10</sub></span> and it won't be <span class="tex-span">0</span>. In any other case the number won't be greater than <span class="tex-span">10<sup class="upper-index">15</sup><sub class="lower-index">10</sub></span>.</p></div><div class="output-specification"><p>Write a single line that contains integer <span class="tex-span"><i>c</i></span> in base <span class="tex-span"><i>b</i></span>. You must omit leading zeros.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">2 ≤ <i>a</i>, <i>b</i> ≤ 25</span>). Only <span class="tex-span"><i>b</i></span> may be replaced by an <span class="tex-font-style-tt">R</span> which indicates Roman numbering system.</p><p>The next line contains a single non-negative integer <span class="tex-span"><i>c</i></span> in base <span class="tex-span"><i>a</i></span> which may contain leading zeros but its length doesn't exceed <span class="tex-span">10<sup class="upper-index">3</sup></span>. </p><p>It is guaranteed that if we have Roman numerals included the number would be less than or equal to <span class="tex-span">3000<sub class="lower-index">10</sub></span> and it won't be <span class="tex-span">0</span>. In any other case the number won't be greater than <span class="tex-span">10<sup class="upper-index">15</sup><sub class="lower-index">10</sub></span>.</p>

## Output

<p>Write a single line that contains integer <span class="tex-span"><i>c</i></span> in base <span class="tex-span"><i>b</i></span>. You must omit leading zeros.</p>





```input1
10 2
1

```




```input2
16 R
5

```




```input3
5 R
4

```




```input4
2 2
1111001

```




```input5
12 13
A

```




```output1
1

```




```output2
V

```




```output3
IV

```




```output4
1111001

```




```output5
A

```



## Note

<p>You can find more information about roman numerals here: http://en.wikipedia.org/wiki/Roman_numerals</p>
