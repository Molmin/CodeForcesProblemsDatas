## Description

<div><p>Sherlock found a piece of encrypted data which he thinks will be useful to catch Moriarty. The encrypted data consists of two integer <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span>. He noticed that these integers were in hexadecimal form.</p><p>He takes each of the integers from <span class="tex-span"><i>l</i></span> to <span class="tex-span"><i>r</i></span>, and performs the following operations:</p><ol><li> He lists the distinct digits present in the given number. For example: for <span class="tex-span">1014<sub class="lower-index">16</sub></span>, he lists the digits as <span class="tex-span">1, 0, 4</span>. </li><li> Then he sums respective powers of two for each digit listed in the step above. Like in the above example <span class="tex-span"><i>sum</i> = 2<sup class="upper-index">1</sup> + 2<sup class="upper-index">0</sup> + 2<sup class="upper-index">4</sup> = 19<sub class="lower-index">10</sub></span>. </li><li> He changes the initial number by applying bitwise <span class="tex-font-style-tt">xor</span> of the initial number and the sum. Example: <img align="middle" class="tex-formula" src="file://ivwW2iZz.png" style="max-width: 100.0%;max-height: 100.0%;">. Note that <span class="tex-font-style-tt">xor</span> is done in binary notation. </li></ol><p>One more example: for integer <span class="tex-font-style-tt">1e</span> the sum is <span class="tex-span"><i>sum</i> = 2<sup class="upper-index">1</sup> + 2<sup class="upper-index">14</sup></span>. Letters <span class="tex-font-style-tt">a</span>, <span class="tex-font-style-tt">b</span>, <span class="tex-font-style-tt">c</span>, <span class="tex-font-style-tt">d</span>, <span class="tex-font-style-tt">e</span>, <span class="tex-font-style-tt">f</span> denote hexadecimal digits <span class="tex-span">10</span>, <span class="tex-span">11</span>, <span class="tex-span">12</span>, <span class="tex-span">13</span>, <span class="tex-span">14</span>, <span class="tex-span">15</span>, respertively.</p><p>Sherlock wants to count the numbers in the range from <span class="tex-span"><i>l</i></span> to <span class="tex-span"><i>r</i></span> (both inclusive) which decrease on application of the above four steps. He wants you to answer his <span class="tex-span"><i>q</i></span> queries for different <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span>.</p></div><div class="input-specification"><p>First line contains the integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10000</span>).</p><p>Each of the next <span class="tex-span"><i>q</i></span> lines contain two hexadecimal integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">0 ≤ <i>l</i> ≤ <i>r</i> &lt; 16<sup class="upper-index">15</sup></span>).</p><p>The hexadecimal integers are written using digits from <span class="tex-span">0</span> to <span class="tex-span">9</span> and/or lowercase English letters <span class="tex-font-style-tt">a</span>, <span class="tex-font-style-tt">b</span>, <span class="tex-font-style-tt">c</span>, <span class="tex-font-style-tt">d</span>, <span class="tex-font-style-tt">e</span>, <span class="tex-font-style-tt">f</span>.</p><p>The hexadecimal integers do not contain extra leading zeros.</p></div><div class="output-specification"><p>Output <span class="tex-span"><i>q</i></span> lines, <span class="tex-span"><i>i</i></span>-th line contains answer to the <span class="tex-span"><i>i</i></span>-th query (in decimal notation).</p></div>

## Input

<p>First line contains the integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10000</span>).</p><p>Each of the next <span class="tex-span"><i>q</i></span> lines contain two hexadecimal integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">0 ≤ <i>l</i> ≤ <i>r</i> &lt; 16<sup class="upper-index">15</sup></span>).</p><p>The hexadecimal integers are written using digits from <span class="tex-span">0</span> to <span class="tex-span">9</span> and/or lowercase English letters <span class="tex-font-style-tt">a</span>, <span class="tex-font-style-tt">b</span>, <span class="tex-font-style-tt">c</span>, <span class="tex-font-style-tt">d</span>, <span class="tex-font-style-tt">e</span>, <span class="tex-font-style-tt">f</span>.</p><p>The hexadecimal integers do not contain extra leading zeros.</p>

## Output

<p>Output <span class="tex-span"><i>q</i></span> lines, <span class="tex-span"><i>i</i></span>-th line contains answer to the <span class="tex-span"><i>i</i></span>-th query (in decimal notation).</p>





```input1
1
1014 1014

```




```input2
2
1 1e
1 f

```




```input3
2
1 abc
d0e fe23

```




```output1
1

```




```output2
1
0

```




```output3
412
28464

```



## Note

<p>For the second input,</p><p><span class="tex-span">14<sub class="lower-index">16</sub> = 20<sub class="lower-index">10</sub></span></p><p><span class="tex-span"><i>sum</i> = 2<sup class="upper-index">1</sup> + 2<sup class="upper-index">4</sup> = 18</span> </p><p><img align="middle" class="tex-formula" src="file://4yzc2D3u.png" style="max-width: 100.0%;max-height: 100.0%;"> </p><p>Thus, it reduces. And, we can verify that it is the only number in range <span class="tex-span">1</span> to <span class="tex-span">1<i>e</i></span> that reduces.</p>
