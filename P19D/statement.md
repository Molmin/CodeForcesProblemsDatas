## Description

<div><p>Pete and Bob invented a new interesting game. Bob takes a sheet of paper and locates a Cartesian coordinate system on it as follows: point <span class="tex-span">(0, 0)</span> is located in the bottom-left corner, <span class="tex-span"><i>Ox</i></span> axis is directed right, <span class="tex-span"><i>Oy</i></span> axis is directed up. Pete gives Bob requests of three types: </p><ul> <li> <span class="tex-font-style-tt">add x y</span> — on the sheet of paper Bob marks a point with coordinates <span class="tex-span">(<i>x</i>, <i>y</i>)</span>. For each request of this type it's guaranteed that point <span class="tex-span">(<i>x</i>, <i>y</i>)</span> is not yet marked on Bob's sheet at the time of the request. </li><li> <span class="tex-font-style-tt">remove x y</span> — on the sheet of paper Bob erases the previously marked point with coordinates <span class="tex-span">(<i>x</i>, <i>y</i>)</span>. For each request of this type it's guaranteed that point <span class="tex-span">(<i>x</i>, <i>y</i>)</span> is already marked on Bob's sheet at the time of the request. </li><li> <span class="tex-font-style-tt">find x y</span> — on the sheet of paper Bob finds all the marked points, lying strictly above and strictly to the right of point <span class="tex-span">(<i>x</i>, <i>y</i>)</span>. Among these points Bob chooses the leftmost one, if it is not unique, he chooses the bottommost one, and gives its coordinates to Pete. </li></ul><p>Bob managed to answer the requests, when they were 10, 100 or 1000, but when their amount grew up to <span class="tex-span">2·10<sup class="upper-index">5</sup></span>, Bob failed to cope. Now he needs a program that will answer all Pete's requests. Help Bob, please!</p></div><div class="input-specification"><p>The first input line contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — amount of requests. Then there follow <span class="tex-span"><i>n</i></span> lines — descriptions of the requests. <span class="tex-font-style-tt">add x y</span> describes the request to add a point, <span class="tex-font-style-tt">remove x y</span> — the request to erase a point, <span class="tex-font-style-tt">find x y</span> — the request to find the bottom-left point. All the coordinates in the input file are non-negative and don't exceed <span class="tex-span">10<sup class="upper-index">9</sup></span>.</p></div><div class="output-specification"><p>For each request of type <span class="tex-font-style-tt">find x y</span> output in a separate line the answer to it — coordinates of the bottommost among the leftmost marked points, lying strictly above and to the right of point <span class="tex-span">(<i>x</i>, <i>y</i>)</span>. If there are no points strictly above and to the right of point <span class="tex-span">(<i>x</i>, <i>y</i>)</span>, output <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>The first input line contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — amount of requests. Then there follow <span class="tex-span"><i>n</i></span> lines — descriptions of the requests. <span class="tex-font-style-tt">add x y</span> describes the request to add a point, <span class="tex-font-style-tt">remove x y</span> — the request to erase a point, <span class="tex-font-style-tt">find x y</span> — the request to find the bottom-left point. All the coordinates in the input file are non-negative and don't exceed <span class="tex-span">10<sup class="upper-index">9</sup></span>.</p>

## Output

<p>For each request of type <span class="tex-font-style-tt">find x y</span> output in a separate line the answer to it — coordinates of the bottommost among the leftmost marked points, lying strictly above and to the right of point <span class="tex-span">(<i>x</i>, <i>y</i>)</span>. If there are no points strictly above and to the right of point <span class="tex-span">(<i>x</i>, <i>y</i>)</span>, output <span class="tex-font-style-tt">-1</span>.</p>





```input1
7
add 1 1
add 3 4
find 0 0
remove 1 1
find 0 0
add 1 1
find 0 0

```




```input2
13
add 5 5
add 5 6
add 5 7
add 6 5
add 6 6
add 6 7
add 7 5
add 7 6
add 7 7
find 6 6
remove 7 7
find 6 6
find 4 4

```




```output1
1 1
3 4
1 1

```




```output2
7 7
-1
5 5

```


