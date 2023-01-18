## Description

<div><p>We'll call an array of <span class="tex-span"><i>n</i></span> non-negative integers <span class="tex-span"><i>a</i>[1], <i>a</i>[2], ..., <i>a</i>[<i>n</i>]</span> <span class="tex-font-style-it">interesting</span>, if it meets <span class="tex-span"><i>m</i></span> constraints. The <span class="tex-span"><i>i</i></span>-th of the <span class="tex-span"><i>m</i></span> constraints consists of three integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) meaning that value <img align="middle" class="tex-formula" src="file://ZtgX39WP.png" style="max-width: 100.0%;max-height: 100.0%;"> should be equal to <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span>. </p><p>Your task is to find any <span class="tex-font-style-it">interesting</span> array of <span class="tex-span"><i>n</i></span> elements or state that such array doesn't exist.</p><p>Expression <span class="tex-span"><i>x</i>&amp;<i>y</i></span> means the bitwise AND of numbers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>. In programming languages C++, Java and Python this operation is represented as "&amp;", in Pascal — as "and".</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of elements in the array and the number of limits.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains three integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>q</i><sub class="lower-index"><i>i</i></sub> &lt; 2<sup class="upper-index">30</sup></span>) describing the <span class="tex-span"><i>i</i></span>-th limit.</p></div><div class="output-specification"><p>If the <span class="tex-font-style-it">interesting</span> array exists, in the first line print "YES" (without the quotes) and in the second line print <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i>[1], <i>a</i>[2], ..., <i>a</i>[<i>n</i>]</span> (<span class="tex-span">0 ≤ <i>a</i>[<i>i</i>] &lt; 2<sup class="upper-index">30</sup></span>)&nbsp;decribing the <span class="tex-font-style-it">interesting</span> array. If there are multiple answers, print any of them.</p><p>If the <span class="tex-font-style-it">interesting</span> array doesn't exist, print "NO" (without the quotes) in the single line.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of elements in the array and the number of limits.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains three integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>q</i><sub class="lower-index"><i>i</i></sub> &lt; 2<sup class="upper-index">30</sup></span>) describing the <span class="tex-span"><i>i</i></span>-th limit.</p>

## Output

<p>If the <span class="tex-font-style-it">interesting</span> array exists, in the first line print "YES" (without the quotes) and in the second line print <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i>[1], <i>a</i>[2], ..., <i>a</i>[<i>n</i>]</span> (<span class="tex-span">0 ≤ <i>a</i>[<i>i</i>] &lt; 2<sup class="upper-index">30</sup></span>)&nbsp;decribing the <span class="tex-font-style-it">interesting</span> array. If there are multiple answers, print any of them.</p><p>If the <span class="tex-font-style-it">interesting</span> array doesn't exist, print "NO" (without the quotes) in the single line.</p>





```input1
3 1
1 3 3

```




```input2
3 2
1 3 3
1 3 2

```




```output1
YES
3 3 3

```




```output2
NO

```


