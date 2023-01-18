## Description

<div><p>Barney is standing in a bar and starring at a pretty girl. He wants to shoot her with his heart arrow but he needs to know the distance between him and the girl to make his shot accurate.</p><center> <img class="tex-graphics" src="file://kQ63XdcD.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Barney asked the bar tender Carl about this distance value, but Carl was so busy talking to the customers so he wrote the distance value (it's a real number) on a napkin. The problem is that he wrote it in scientific notation. The scientific notation of some real number <span class="tex-span"><i>x</i></span> is the notation of form <span class="tex-span"><i>AeB</i></span>, where <span class="tex-span"><i>A</i></span> is a real number and <span class="tex-span"><i>B</i></span> is an integer and <span class="tex-span"><i>x</i> = <i>A</i> × 10<sup class="upper-index"><i>B</i></sup></span> is true. In our case <span class="tex-span"><i>A</i></span> is between <span class="tex-span">0</span> and <span class="tex-span">9</span> and <span class="tex-span"><i>B</i></span> is non-negative.</p><p>Barney doesn't know anything about scientific notation (as well as anything scientific at all). So he asked you to tell him the distance value in usual decimal representation with minimal number of digits after the decimal point (and no decimal point if it is an integer). See the output format for better understanding.</p></div><div class="input-specification"><p>The first and only line of input contains a single string of form <span class="tex-span"><i>a</i>.<i>deb</i></span> where <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>d</i></span> and <span class="tex-span"><i>b</i></span> are integers and <span class="tex-span"><i>e</i></span> is usual character 'e' (<span class="tex-span">0 ≤ <i>a</i> ≤ 9, 0 ≤ <i>d</i> &lt; 10<sup class="upper-index">100</sup>, 0 ≤ <i>b</i> ≤ 100</span>)&nbsp;— the scientific notation of the desired distance value.</p><p><span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> contain no leading zeros and <span class="tex-span"><i>d</i></span> contains no trailing zeros (but may be equal to <span class="tex-span">0</span>). Also, <span class="tex-font-style-bf"><span class="tex-span"><i>b</i></span> can not be non-zero if <span class="tex-span"><i>a</i></span> is zero.</span></p></div><div class="output-specification"><p>Print the only real number <span class="tex-span"><i>x</i></span> (the desired distance value) in the only line in its decimal notation. </p><p>Thus if <span class="tex-span"><i>x</i></span> is an integer, print it's integer value without decimal part and decimal point and without leading zeroes. </p><p>Otherwise print <span class="tex-span"><i>x</i></span> in a form of <span class="tex-span"><i>p</i>.<i>q</i></span> such that <span class="tex-span"><i>p</i></span> is an integer that have no leading zeroes (but may be equal to zero), and <span class="tex-span"><i>q</i></span> is an integer that have no trailing zeroes (and may not be equal to zero).</p></div>

## Input

<p>The first and only line of input contains a single string of form <span class="tex-span"><i>a</i>.<i>deb</i></span> where <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>d</i></span> and <span class="tex-span"><i>b</i></span> are integers and <span class="tex-span"><i>e</i></span> is usual character 'e' (<span class="tex-span">0 ≤ <i>a</i> ≤ 9, 0 ≤ <i>d</i> &lt; 10<sup class="upper-index">100</sup>, 0 ≤ <i>b</i> ≤ 100</span>)&nbsp;— the scientific notation of the desired distance value.</p><p><span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> contain no leading zeros and <span class="tex-span"><i>d</i></span> contains no trailing zeros (but may be equal to <span class="tex-span">0</span>). Also, <span class="tex-font-style-bf"><span class="tex-span"><i>b</i></span> can not be non-zero if <span class="tex-span"><i>a</i></span> is zero.</span></p>

## Output

<p>Print the only real number <span class="tex-span"><i>x</i></span> (the desired distance value) in the only line in its decimal notation. </p><p>Thus if <span class="tex-span"><i>x</i></span> is an integer, print it's integer value without decimal part and decimal point and without leading zeroes. </p><p>Otherwise print <span class="tex-span"><i>x</i></span> in a form of <span class="tex-span"><i>p</i>.<i>q</i></span> such that <span class="tex-span"><i>p</i></span> is an integer that have no leading zeroes (but may be equal to zero), and <span class="tex-span"><i>q</i></span> is an integer that have no trailing zeroes (and may not be equal to zero).</p>





```input1
8.549e2

```




```input2
8.549e3

```




```input3
0.33e0

```




```output1
854.9

```




```output2
8549

```




```output3
0.33

```


