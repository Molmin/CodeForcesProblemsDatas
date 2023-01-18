## Description

<div><p>Igor likes hexadecimal notation and considers <span class="tex-font-style-bf">positive</span> integer in the hexadecimal notation <span class="tex-font-style-it">interesting</span> if each digit and each letter in it appears no more than <span class="tex-span"><i>t</i></span> times. For example, if <span class="tex-span"><i>t</i> = 3</span>, then integers <span class="tex-font-style-tt">13a13322</span>, <span class="tex-font-style-tt">aaa</span>, <span class="tex-font-style-tt">abcdef0123456789</span> are interesting, but numbers <span class="tex-font-style-tt">aaaa</span>, <span class="tex-font-style-tt">abababab</span> and <span class="tex-font-style-tt">1000000</span> are not interesting.</p><p>Your task is to find the <span class="tex-span"><i>k</i></span>-th smallest <span class="tex-font-style-it">interesting</span> for Igor integer in the hexadecimal notation. The integer should not contain leading zeros.</p></div><div class="input-specification"><p>The first line contains the two integers <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 2·10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>t</i> ≤ 10</span>) — the number of the required integer and the maximum number of times some integer or letter can appear in interesting integer.</p><p>It can be shown that the answer always exists for such constraints.</p></div><div class="output-specification"><p>Print in the hexadecimal notation the only integer that is the <span class="tex-span"><i>k</i></span>-th smallest <span class="tex-font-style-it">interesting</span> integer for Igor.</p></div>

## Input

<p>The first line contains the two integers <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 2·10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>t</i> ≤ 10</span>) — the number of the required integer and the maximum number of times some integer or letter can appear in interesting integer.</p><p>It can be shown that the answer always exists for such constraints.</p>

## Output

<p>Print in the hexadecimal notation the only integer that is the <span class="tex-span"><i>k</i></span>-th smallest <span class="tex-font-style-it">interesting</span> integer for Igor.</p>





```input1
17 1

```




```input2
1000000 2

```




```output1
12

```




```output2
fca2c

```



## Note

<p>The first 20 <span class="tex-font-style-it">interesting</span> integers if <span class="tex-span"><i>t</i> = 1</span>: <span class="tex-font-style-tt">1</span>, <span class="tex-font-style-tt">2</span>, <span class="tex-font-style-tt">3</span>, <span class="tex-font-style-tt">4</span>, <span class="tex-font-style-tt">5</span>, <span class="tex-font-style-tt">6</span>, <span class="tex-font-style-tt">7</span>, <span class="tex-font-style-tt">8</span>, <span class="tex-font-style-tt">9</span>, <span class="tex-font-style-tt">a</span>, <span class="tex-font-style-tt">b</span>, <span class="tex-font-style-tt">c</span>, <span class="tex-font-style-tt">d</span>, <span class="tex-font-style-tt">e</span>, <span class="tex-font-style-tt">f</span>, <span class="tex-font-style-tt">10</span>, <span class="tex-font-style-tt">12</span>, <span class="tex-font-style-tt">13</span>, <span class="tex-font-style-tt">14</span>, <span class="tex-font-style-tt">15</span>. So the answer for the first example equals <span class="tex-font-style-tt">12</span>.</p>
