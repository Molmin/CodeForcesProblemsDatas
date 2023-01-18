## Description

<div><p>Sherlock Holmes and Dr. Watson played some game on a checkered board <span class="tex-span"><i>n</i> × <i>n</i></span> in size. During the game they put numbers on the board's squares by some tricky rules we don't know. However, the game is now over and each square of the board contains exactly one number. To understand who has won, they need to count the number of <span class="tex-font-style-underline">winning</span> squares. To determine if the particular square is winning you should do the following. Calculate the sum of all numbers on the squares that share this column (including the given square) and separately calculate the sum of all numbers on the squares that share this row (including the given square). A square is considered <span class="tex-font-style-underline">winning</span> if the sum of the column numbers is <span class="tex-font-style-bf">strictly</span> greater than the sum of the row numbers.</p><center><img class="tex-graphics" src="file://PuzoZz8y.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>For instance, lets game was ended like is shown in the picture. Then the purple cell is winning, because the sum of its column numbers equals <span class="tex-span">8 + 3 + 6 + 7 = 24</span>, sum of its row numbers equals <span class="tex-span">9 + 5 + 3 + 2 = 19</span>, and <span class="tex-span">24 &gt; 19</span>.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 30</span>). Each of the following <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>n</i></span> space-separated integers. The <span class="tex-span"><i>j</i></span>-th number on the <span class="tex-span"><i>i</i></span>-th line represents the number on the square that belongs to the <span class="tex-span"><i>j</i></span>-th column and the <span class="tex-span"><i>i</i></span>-th row on the board. All number on the board are integers from <span class="tex-span">1</span> to <span class="tex-span">100</span>.</p></div><div class="output-specification"><p>Print the single number — the number of the winning squares.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 30</span>). Each of the following <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>n</i></span> space-separated integers. The <span class="tex-span"><i>j</i></span>-th number on the <span class="tex-span"><i>i</i></span>-th line represents the number on the square that belongs to the <span class="tex-span"><i>j</i></span>-th column and the <span class="tex-span"><i>i</i></span>-th row on the board. All number on the board are integers from <span class="tex-span">1</span> to <span class="tex-span">100</span>.</p>

## Output

<p>Print the single number — the number of the winning squares.</p>





```input1
1
1

```




```input2
2
1 2
3 4

```




```input3
4
5 7 8 4
9 5 3 2
1 6 6 4
9 5 7 3

```




```output1
0

```




```output2
2

```




```output3
6

```



## Note

<p>In the first example two upper squares are winning.</p><p>In the third example three left squares in the both middle rows are winning:</p><pre class="verbatim">5 7 8 4<br><span class="tex-font-style-bf"><span class="tex-font-style-underline"><span class="tex-span">9</span> <span class="tex-span">5</span> <span class="tex-span">3</span></span></span> 2<br><span class="tex-font-style-bf"><span class="tex-font-style-underline"><span class="tex-span">1</span> <span class="tex-span">6</span> <span class="tex-span">6</span></span></span> 4<br>9 5 7 3<br></pre>
