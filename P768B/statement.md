## Description

<div><p>Jon fought bravely to rescue the wildlings who were attacked by the white-walkers at Hardhome. On his arrival, Sam tells him that he wants to go to Oldtown to train at the Citadel to become a maester, so he can return and take the deceased Aemon's place as maester of Castle Black. Jon agrees to Sam's proposal and Sam sets off his journey to the Citadel. However becoming a trainee at the Citadel is not a cakewalk and hence the maesters at the Citadel gave Sam a problem to test his eligibility. </p><p>Initially Sam has a list with a single element <span class="tex-span"><i>n</i></span>. Then he has to perform certain operations on this list. In each operation Sam must remove any element <span class="tex-span"><i>x</i></span>, such that <span class="tex-span"><i>x</i> &gt; 1</span>, from the list and insert at the same position <img align="middle" class="tex-formula" src="file://g6joDXXi.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://Dd0oWuRz.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://0sk5Uxec.png" style="max-width: 100.0%;max-height: 100.0%;"> sequentially. He must continue with these operations until all the elements in the list are either <span class="tex-span">0</span> or <span class="tex-span">1</span>.</p><p>Now the masters want the total number of <span class="tex-span">1</span>s in the range <span class="tex-span"><i>l</i></span> to <span class="tex-span"><i>r</i></span> (<span class="tex-span">1</span>-indexed). Sam wants to become a maester but unfortunately he cannot solve this problem. Can you help Sam to pass the eligibility test?</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span> (<span class="tex-span">0 ≤ <i>n</i> &lt; 2<sup class="upper-index">50</sup></span>, <span class="tex-span">0 ≤ <i>r</i> - <i>l</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span"><i>r</i> ≥ 1</span>, <span class="tex-span"><i>l</i> ≥ 1</span>) – initial element and the range <span class="tex-span"><i>l</i></span> to <span class="tex-span"><i>r</i></span>.</p><p>It is guaranteed that <span class="tex-span"><i>r</i></span> is not greater than the length of the final list.</p></div><div class="output-specification"><p>Output the total number of <span class="tex-span">1</span>s in the range <span class="tex-span"><i>l</i></span> to <span class="tex-span"><i>r</i></span> in the final sequence.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span> (<span class="tex-span">0 ≤ <i>n</i> &lt; 2<sup class="upper-index">50</sup></span>, <span class="tex-span">0 ≤ <i>r</i> - <i>l</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span"><i>r</i> ≥ 1</span>, <span class="tex-span"><i>l</i> ≥ 1</span>) – initial element and the range <span class="tex-span"><i>l</i></span> to <span class="tex-span"><i>r</i></span>.</p><p>It is guaranteed that <span class="tex-span"><i>r</i></span> is not greater than the length of the final list.</p>

## Output

<p>Output the total number of <span class="tex-span">1</span>s in the range <span class="tex-span"><i>l</i></span> to <span class="tex-span"><i>r</i></span> in the final sequence.</p>





```input1
7 2 5

```




```input2
10 3 10

```




```output1
4

```




```output2
5

```



## Note

<p>Consider first example:</p><p><img align="middle" class="tex-formula" src="file://vYQP4AoZ.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>Elements on positions from <span class="tex-span">2</span>-nd to <span class="tex-span">5</span>-th in list is <span class="tex-span">[1, 1, 1, 1]</span>. The number of ones is <span class="tex-span">4</span>.</p><p>For the second example:</p><p><img align="middle" class="tex-formula" src="file://Eg5A7Gdl.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>Elements on positions from <span class="tex-span">3</span>-rd to <span class="tex-span">10</span>-th in list is <span class="tex-span">[1, 1, 1, 0, 1, 0, 1, 0]</span>. The number of ones is <span class="tex-span">5</span>.</p>
