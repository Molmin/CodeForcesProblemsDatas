## Description

<div><p>The Floral Clock has been standing by the side of Mirror Lake for years. Though unable to keep time, it reminds people of the passage of time and the good old days.</p><p>On the rim of the Floral Clock are <span class="tex-span">2<i>n</i></span> flowers, numbered from <span class="tex-span">1</span> to <span class="tex-span">2<i>n</i></span> clockwise, each of which has a colour among all <span class="tex-span"><i>n</i></span> possible ones. For each colour, there are exactly two flowers with it, the <span class="tex-font-style-underline">distance</span> between which <span class="tex-font-style-bf">either is less than or equal to <span class="tex-span">2</span>, or equals <span class="tex-span"><i>n</i></span></span>. Additionally, if flowers <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> are of the same colour, then flowers opposite to <span class="tex-span"><i>u</i></span> and opposite to <span class="tex-span"><i>v</i></span> should be of the same colour as well — symmetry is beautiful!</p><p>Formally, the <span class="tex-font-style-underline">distance</span> between two flowers is <span class="tex-span">1</span> plus the number of flowers on the minor arc (or semicircle) between them. Below is a possible arrangement with <span class="tex-span"><i>n</i> = 6</span> that cover all possibilities.</p><center> <img class="tex-graphics" src="file://z75f1yeP.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The <span class="tex-font-style-underline">beauty</span> of an arrangement is defined to be the product of the lengths of flower segments separated by all opposite flowers of the same colour. In other words, in order to compute the beauty, we remove from the circle all flowers that have the same colour as flowers opposite to them. Then, the beauty is the product of lengths of all remaining segments. Note that we include segments of length <span class="tex-span">0</span> in this product. If there are no flowers that have the same colour as flower opposite to them, the beauty equals <span class="tex-span">0</span>. For instance, the <span class="tex-font-style-underline">beauty</span> of the above arrangement equals <span class="tex-span">1 × 3 × 1 × 3 = 9</span> — the segments are <span class="tex-span">{2}</span>, <span class="tex-span">{4, 5, 6}</span>, <span class="tex-span">{8}</span> and <span class="tex-span">{10, 11, 12}</span>.</p><p>While keeping the constraints satisfied, there may be lots of different arrangements. Find out the sum of <span class="tex-font-style-underline">beauty</span> over all possible arrangements, modulo <span class="tex-span">998 244 353</span>. Two arrangements are considered different, if a pair <span class="tex-span">(<i>u</i>, <i>v</i>)</span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ 2<i>n</i></span>) exists such that flowers <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> are of the same colour in one of them, but not in the other.</p></div><div class="input-specification"><p>The first and only line of input contains a lonely positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 50 000</span>)&nbsp;— the number of colours present on the Floral Clock.</p></div><div class="output-specification"><p>Output one integer — the sum of <span class="tex-font-style-underline">beauty</span> over all possible arrangements of flowers, modulo <span class="tex-span">998 244 353</span>.</p></div>

## Input

<p>The first and only line of input contains a lonely positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 50 000</span>)&nbsp;— the number of colours present on the Floral Clock.</p>

## Output

<p>Output one integer — the sum of <span class="tex-font-style-underline">beauty</span> over all possible arrangements of flowers, modulo <span class="tex-span">998 244 353</span>.</p>





```input1
3

```




```input2
4

```




```input3
7

```




```input4
15

```




```output1
24

```




```output2
4

```




```output3
1316

```




```output4
3436404

```



## Note

<p>With <span class="tex-span"><i>n</i> = 3</span>, the following six arrangements each have a <span class="tex-font-style-underline">beauty</span> of <span class="tex-span">2 × 2 = 4</span>.</p><center> <img class="tex-graphics" src="file://GMMmRf0t.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>While many others, such as the left one in the figure below, have a <span class="tex-font-style-underline">beauty</span> of <span class="tex-span">0</span>. The right one is invalid, since it's asymmetric.</p><center> <img class="tex-graphics" src="file://kntffGSN.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
