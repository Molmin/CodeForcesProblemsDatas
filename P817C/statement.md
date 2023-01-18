## Description

<div><p>Ivan likes to learn different things about numbers, but he is especially interested in <span class="tex-font-style-it">really big</span> numbers. Ivan thinks that a positive integer number <span class="tex-span"><i>x</i></span> is <span class="tex-font-style-it">really big</span> if the difference between <span class="tex-span"><i>x</i></span> and the sum of its digits (in decimal representation) is not less than <span class="tex-span"><i>s</i></span>. To prove that these numbers may have different special properties, he wants to know how rare (or not rare) they are — in fact, he needs to calculate the quantity of <span class="tex-font-style-it">really big</span> numbers that are not greater than <span class="tex-span"><i>n</i></span>.</p><p>Ivan tried to do the calculations himself, but soon realized that it's too difficult for him. So he asked you to help him in calculations.</p></div><div class="input-specification"><p>The first (and the only) line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>s</i> ≤ 10<sup class="upper-index">18</sup></span>).</p></div><div class="output-specification"><p>Print one integer — the quantity of <span class="tex-font-style-it">really big</span> numbers that are not greater than <span class="tex-span"><i>n</i></span>.</p></div>

## Input

<p>The first (and the only) line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>s</i> ≤ 10<sup class="upper-index">18</sup></span>).</p>

## Output

<p>Print one integer — the quantity of <span class="tex-font-style-it">really big</span> numbers that are not greater than <span class="tex-span"><i>n</i></span>.</p>





```input1
12 1

```




```input2
25 20

```




```input3
10 9

```




```output1
3

```




```output2
0

```




```output3
1

```



## Note

<p>In the first example numbers <span class="tex-span">10</span>, <span class="tex-span">11</span> and <span class="tex-span">12</span> are <span class="tex-font-style-it">really big</span>.</p><p>In the second example there are no <span class="tex-font-style-it">really big</span> numbers that are not greater than <span class="tex-span">25</span> (in fact, the first <span class="tex-font-style-it">really big</span> number is <span class="tex-span">30</span>: <span class="tex-span">30 - 3 ≥ 20</span>).</p><p>In the third example <span class="tex-span">10</span> is the only <span class="tex-font-style-it">really big</span> number (<span class="tex-span">10 - 1 ≥ 9</span>).</p>
