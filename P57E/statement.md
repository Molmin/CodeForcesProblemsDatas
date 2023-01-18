## Description

<div><p>Brian the Rabbit adores chess. Not long ago he argued with Stewie the Rabbit that a knight is better than a king. To prove his point he tries to show that the knight is very fast but Stewie doesn't accept statements without evidence. He constructed an infinite chessboard for Brian, where he deleted several squares to add some more interest to the game. Brian only needs to count how many different board squares a knight standing on a square with coordinates of <span class="tex-span">(0, 0)</span> can reach in no more than <span class="tex-span"><i>k</i></span> moves. Naturally, it is forbidden to move to the deleted squares.</p><p>Brian doesn't very much like exact sciences himself and is not acquainted with programming, that's why he will hardly be able to get ahead of Stewie who has already started solving the problem. Help Brian to solve the problem faster than Stewie.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>n</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 10<sup class="upper-index">18</sup>, 0 ≤ <i>n</i> ≤ 440</span>) which are correspondingly the maximal number of moves a knight can make and the number of deleted cells. Then follow <span class="tex-span"><i>n</i></span> lines, each giving the coordinates of a deleted square in the form <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> (<span class="tex-span">|<i>x</i><sub class="lower-index"><i>i</i></sub>| ≤ 10, |<i>y</i><sub class="lower-index"><i>i</i></sub>| ≤ 10</span>). All the numbers are integer, the deleted squares are different and it is guaranteed that the square <span class="tex-span">(0, 0)</span> is not deleted.</p><p>Please, do not use <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is preffered to use <span class="tex-font-style-tt">cin</span> (also you may use <span class="tex-font-style-tt">%I64d</span>).</p></div><div class="output-specification"><p>You must print the answer on a single line. As it can be rather long, you should print it modulo <span class="tex-span">1000000007</span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>n</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 10<sup class="upper-index">18</sup>, 0 ≤ <i>n</i> ≤ 440</span>) which are correspondingly the maximal number of moves a knight can make and the number of deleted cells. Then follow <span class="tex-span"><i>n</i></span> lines, each giving the coordinates of a deleted square in the form <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> (<span class="tex-span">|<i>x</i><sub class="lower-index"><i>i</i></sub>| ≤ 10, |<i>y</i><sub class="lower-index"><i>i</i></sub>| ≤ 10</span>). All the numbers are integer, the deleted squares are different and it is guaranteed that the square <span class="tex-span">(0, 0)</span> is not deleted.</p><p>Please, do not use <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is preffered to use <span class="tex-font-style-tt">cin</span> (also you may use <span class="tex-font-style-tt">%I64d</span>).</p>

## Output

<p>You must print the answer on a single line. As it can be rather long, you should print it modulo <span class="tex-span">1000000007</span>.</p>





```input1
1 0

```




```input2
2 7
-1 2
1 2
2 1
2 -1
1 -2
-1 -2
-2 -1

```




```output1
9

```




```output2
9

```


