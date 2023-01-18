## Description

<div><p>Vasya has become interested in wrestling. In wrestling wrestlers use techniques for which they are awarded points by judges. The wrestler who gets the most points wins.</p><p>When the numbers of points of both wrestlers are equal, the wrestler whose sequence of points is <span class="tex-font-style-bf">lexicographically greater</span>, wins.</p><p>If the sequences of the awarded points coincide, the wrestler who performed the last technique wins. Your task is to determine which wrestler won.</p></div><div class="input-specification"><p>The first line contains number <span class="tex-span"><i>n</i></span> — the number of techniques that the wrestlers have used (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>). </p><p>The following <span class="tex-span"><i>n</i></span> lines contain integer numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">|<i>a</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ 0</span>). If <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is positive, that means that the first wrestler performed the technique that was awarded with <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> points. And if <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is negative, that means that the second wrestler performed the technique that was awarded with <span class="tex-span">( - <i>a</i><sub class="lower-index"><i>i</i></sub>)</span> points.</p><p>The techniques are given in chronological order.</p></div><div class="output-specification"><p>If the first wrestler wins, print string "<span class="tex-font-style-tt">first</span>", otherwise print "<span class="tex-font-style-tt">second</span>"</p></div>

## Input

<p>The first line contains number <span class="tex-span"><i>n</i></span> — the number of techniques that the wrestlers have used (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>). </p><p>The following <span class="tex-span"><i>n</i></span> lines contain integer numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">|<i>a</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ 0</span>). If <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is positive, that means that the first wrestler performed the technique that was awarded with <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> points. And if <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is negative, that means that the second wrestler performed the technique that was awarded with <span class="tex-span">( - <i>a</i><sub class="lower-index"><i>i</i></sub>)</span> points.</p><p>The techniques are given in chronological order.</p>

## Output

<p>If the first wrestler wins, print string "<span class="tex-font-style-tt">first</span>", otherwise print "<span class="tex-font-style-tt">second</span>"</p>





```input1
5
1
2
-3
-4
3

```




```input2
3
-1
-2
3

```




```input3
2
4
-4

```




```output1
second

```




```output2
first

```




```output3
second

```



## Note

<p>Sequence <span class="tex-span"><i>x</i>  =  <i>x</i><sub class="lower-index">1</sub><i>x</i><sub class="lower-index">2</sub>... <i>x</i><sub class="lower-index">|<i>x</i>|</sub></span> is <span class="tex-font-style-bf">lexicographically larger</span> than sequence <span class="tex-span"><i>y</i>  =  <i>y</i><sub class="lower-index">1</sub><i>y</i><sub class="lower-index">2</sub>... <i>y</i><sub class="lower-index">|<i>y</i>|</sub></span>, if either <span class="tex-span">|<i>x</i>|  &gt;  |<i>y</i>|</span> and <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>  =  <i>y</i><sub class="lower-index">1</sub>,  <i>x</i><sub class="lower-index">2</sub>  =  <i>y</i><sub class="lower-index">2</sub>, ... ,  <i>x</i><sub class="lower-index">|<i>y</i>|</sub>  =  <i>y</i><sub class="lower-index">|<i>y</i>|</sub></span>, or there is such number <span class="tex-span"><i>r</i></span> (<span class="tex-span"><i>r</i>  &lt;  |<i>x</i>|</span>, <span class="tex-span"><i>r</i>  &lt;  |<i>y</i>|</span>), that <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>  =  <i>y</i><sub class="lower-index">1</sub>,  <i>x</i><sub class="lower-index">2</sub>  =  <i>y</i><sub class="lower-index">2</sub>,  ... ,  <i>x</i><sub class="lower-index"><i>r</i></sub>  =  <i>y</i><sub class="lower-index"><i>r</i></sub></span> and <span class="tex-span"><i>x</i><sub class="lower-index"><i>r</i>  +  1</sub>  &gt;  <i>y</i><sub class="lower-index"><i>r</i>  +  1</sub></span>.</p><p>We use notation <span class="tex-span">|<i>a</i>|</span> to denote length of sequence <span class="tex-span"><i>a</i></span>.</p>
