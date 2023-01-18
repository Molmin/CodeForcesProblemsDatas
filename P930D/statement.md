## Description

<div><p>Consider the following game for two players. There is one white token and some number of black tokens. Each token is placed on a plane in a point with integer coordinates <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>.</p><p>The players take turn making moves, white starts. On each turn, a player moves <span class="tex-font-style-bf">all</span> tokens of their color by <span class="tex-span">1</span> to up, down, left or right. Black player can choose directions for each token independently.</p><p>After a turn of the white player the white token can not be in a point where a black token is located. There are no other constraints on locations of the tokens: positions of black tokens can coincide, after a turn of the black player and initially the white token can be in the same point with some black point. If at some moment the white player can't make a move, he loses. If the white player makes <span class="tex-span">10<sup class="upper-index">100500</sup></span> moves, he wins.</p><p>You are to solve the following problem. You are given initial positions of all black tokens. It is guaranteed that initially all these positions are distinct. In how many places can the white token be located initially so that if both players play optimally, the black player wins?</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of black points.</p><p>The (<span class="tex-span"><i>i</i> + 1</span>)-th line contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">5</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>,  ≤ 10<sup class="upper-index">5</sup></span>) — the coordinates of the point where the <span class="tex-span"><i>i</i></span>-th black token is initially located.</p><p>It is guaranteed that initial positions of black tokens are distinct.</p></div><div class="output-specification"><p>Print the number of points where the white token can be located initially, such that if both players play optimally, the black player wins.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of black points.</p><p>The (<span class="tex-span"><i>i</i> + 1</span>)-th line contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">5</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>,  ≤ 10<sup class="upper-index">5</sup></span>) — the coordinates of the point where the <span class="tex-span"><i>i</i></span>-th black token is initially located.</p><p>It is guaranteed that initial positions of black tokens are distinct.</p>

## Output

<p>Print the number of points where the white token can be located initially, such that if both players play optimally, the black player wins.</p>





```input1
4
-2 -1
0 1
0 -3
2 -1

```




```input2
4
-2 0
-1 1
0 -2
1 -1

```




```input3
16
2 1
1 2
-1 1
0 1
0 0
1 1
2 -1
2 0
1 0
-1 -1
1 -1
2 2
0 -1
-1 0
0 2
-1 2

```




```output1
4

```




```output2
2

```




```output3
4

```



## Note

<p>In the first and second examples initial positions of black tokens are shown with black points, possible positions of the white token (such that the black player wins) are shown with white points.</p><p>The first example: <img class="tex-graphics" src="file://kTmAnjcP.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>The second example: <img class="tex-graphics" src="file://EGZ3ygft.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>In the third example the white tokens should be located in the inner square <span class="tex-span">2 × 2</span>, to make the black player win. <img class="tex-graphics" src="file://eFnmzmE8.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
