## Description

<div><p>Vanya walks late at night along a straight street of length <span class="tex-span"><i>l</i></span>, lit by <span class="tex-span"><i>n</i></span> lanterns. Consider the coordinate system with the beginning of the street corresponding to the point <span class="tex-span">0</span>, and its end corresponding to the point <span class="tex-span"><i>l</i></span>. Then the <span class="tex-span"><i>i</i></span>-th lantern is at the point <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. The lantern lights all points of the street that are at the distance of at most <span class="tex-span"><i>d</i></span> from it, where <span class="tex-span"><i>d</i></span> is some positive number, common for all lanterns. </p><p>Vanya wonders: what is the minimum light radius <span class="tex-span"><i>d</i></span> should the lanterns have to light the whole street?</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>l</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>l</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of lanterns and the length of the street respectively. </p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>l</i></span>). Multiple lanterns can be located at the same point. The lanterns may be located at the ends of the street.</p></div><div class="output-specification"><p>Print the minimum light radius <span class="tex-span"><i>d</i></span>, needed to light the whole street. The answer will be considered correct if its absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>l</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>l</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of lanterns and the length of the street respectively. </p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>l</i></span>). Multiple lanterns can be located at the same point. The lanterns may be located at the ends of the street.</p>

## Output

<p>Print the minimum light radius <span class="tex-span"><i>d</i></span>, needed to light the whole street. The answer will be considered correct if its absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p>





```input1
7 15
15 5 3 7 9 14 0

```




```input2
2 5
2 5

```




```output1
2.5000000000

```




```output2
2.0000000000

```



## Note

<p>Consider the second sample. At <span class="tex-span"><i>d</i> = 2</span> the first lantern will light the segment <span class="tex-span">[0, 4]</span> of the street, and the second lantern will light segment <span class="tex-span">[3, 5]</span>. Thus, the whole street will be lit.</p>
