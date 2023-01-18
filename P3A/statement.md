## Description

<div><p>The king is left alone on the chessboard. In spite of this loneliness, he doesn't lose heart, because he has business of national importance. For example, he has to pay an official visit to square <span class="tex-span"><i>t</i></span>. As the king is not in habit of wasting his time, he wants to get from his current position <span class="tex-span"><i>s</i></span> to square <span class="tex-span"><i>t</i></span> in the least number of moves. Help him to do this.</p><center> <img class="tex-graphics" src="file://UzqfgUwQ.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In one move the king can get to the square that has a common side or a common vertex with the square the king is currently in (generally there are 8 different squares he can move to).</p></div><div class="input-specification"><p>The first line contains the chessboard coordinates of square <span class="tex-span"><i>s</i></span>, the second line — of square <span class="tex-span"><i>t</i></span>.</p><p>Chessboard coordinates consist of two characters, the first one is a lowercase Latin letter (from <span class="tex-font-style-tt">a</span> to <span class="tex-font-style-tt">h</span>), the second one is a digit from <span class="tex-font-style-tt">1</span> to <span class="tex-font-style-tt">8</span>.</p></div><div class="output-specification"><p>In the first line print <span class="tex-span"><i>n</i></span> — minimum number of the king's moves. Then in <span class="tex-span"><i>n</i></span> lines print the moves themselves. Each move is described with one of the 8: <span class="tex-font-style-tt">L</span>, <span class="tex-font-style-tt">R</span>, <span class="tex-font-style-tt">U</span>, <span class="tex-font-style-tt">D</span>, <span class="tex-font-style-tt">LU</span>, <span class="tex-font-style-tt">LD</span>, <span class="tex-font-style-tt">RU</span> or <span class="tex-font-style-tt">RD</span>. </p><p><span class="tex-font-style-tt">L</span>, <span class="tex-font-style-tt">R</span>, <span class="tex-font-style-tt">U</span>, <span class="tex-font-style-tt">D</span> stand respectively for moves left, right, up and down (according to the picture), and 2-letter combinations stand for diagonal moves. If the answer is not unique, print any of them. </p></div>

## Input

<p>The first line contains the chessboard coordinates of square <span class="tex-span"><i>s</i></span>, the second line — of square <span class="tex-span"><i>t</i></span>.</p><p>Chessboard coordinates consist of two characters, the first one is a lowercase Latin letter (from <span class="tex-font-style-tt">a</span> to <span class="tex-font-style-tt">h</span>), the second one is a digit from <span class="tex-font-style-tt">1</span> to <span class="tex-font-style-tt">8</span>.</p>

## Output

<p>In the first line print <span class="tex-span"><i>n</i></span> — minimum number of the king's moves. Then in <span class="tex-span"><i>n</i></span> lines print the moves themselves. Each move is described with one of the 8: <span class="tex-font-style-tt">L</span>, <span class="tex-font-style-tt">R</span>, <span class="tex-font-style-tt">U</span>, <span class="tex-font-style-tt">D</span>, <span class="tex-font-style-tt">LU</span>, <span class="tex-font-style-tt">LD</span>, <span class="tex-font-style-tt">RU</span> or <span class="tex-font-style-tt">RD</span>. </p><p><span class="tex-font-style-tt">L</span>, <span class="tex-font-style-tt">R</span>, <span class="tex-font-style-tt">U</span>, <span class="tex-font-style-tt">D</span> stand respectively for moves left, right, up and down (according to the picture), and 2-letter combinations stand for diagonal moves. If the answer is not unique, print any of them. </p>





```input1
a8
h1

```




```output1
7
RD
RD
RD
RD
RD
RD
RD

```


