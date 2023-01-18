## Description

<div><p>Andryusha has found a perplexing arcade machine. The machine is a vertically adjusted board divided into square cells. The board has <span class="tex-span"><i>w</i></span> columns numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>w</i></span> from left to right, and <span class="tex-span"><i>h</i></span> rows numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>h</i></span> from the bottom to the top.</p><p>Further, there are barriers in some of board rows. There are <span class="tex-span"><i>n</i></span> barriers in total, and <span class="tex-span"><i>i</i></span>-th of them occupied the cells <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> through <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> of the row <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>. Andryusha recollects well that no two barriers share the same row. Furthermore, no row is completely occupied with a barrier, that is, at least one cell in each row is free.</p><p>The player can throw a marble to any column of the machine from above. A marble falls downwards until it encounters a barrier, or falls through the bottom of the board. A marble disappears once it encounters a barrier but is replaced by two more marbles immediately to the left and to the right of the same barrier. In a situation when the barrier is at an edge of the board, both marbles appear next to the barrier at the side opposite to the edge. More than one marble can occupy the same place of the board, without obstructing each other's movement. Ultimately, all marbles are bound to fall from the bottom of the machine.</p><center> <img class="tex-graphics" height="265px" src="file://J2eu6WAL.png" style="max-width: 100.0%;max-height: 100.0%;" width="378px">   <span class="tex-font-size-small">Examples of marble-barrier interaction.</span> </center><p>Peculiarly, sometimes marbles can go through barriers as if they were free cells. That is so because the barriers are in fact alive, and frightened when a marble was coming at them from a very high altitude. More specifically, if a marble falls towards the barrier <span class="tex-span"><i>i</i></span> from relative height more than <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> (that is, it started its fall strictly higher than <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub> + <i>s</i><sub class="lower-index"><i>i</i></sub></span>), then the barrier evades the marble. If a marble is thrown from the top of the board, it is considered to appear at height <span class="tex-span">(<i>h</i> + 1)</span>.</p><p>Andryusha remembers to have thrown a marble once in each of the columns. Help him find the total number of marbles that came down at the bottom of the machine. Since the answer may be large, print it modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>h</i></span>, <span class="tex-span"><i>w</i></span>, and <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>h</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">2 ≤ <i>w</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of rows, columns, and barriers in the machine respectively.</p><p>Next <span class="tex-span"><i>n</i></span> lines describe barriers. <span class="tex-span"><i>i</i></span>-th of these lines containts four integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>, and <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub> ≤ <i>h</i></span>, <span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>w</i></span>, <span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— row index, leftmost and rightmost column index of <span class="tex-span"><i>i</i></span>-th barrier, and largest relative fall height such that the barrier does not evade a falling marble. It is guaranteed that each row has at least one free cell, and that all <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> are distinct.</p></div><div class="output-specification"><p>Print one integer&nbsp;— the answer to the problem modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>h</i></span>, <span class="tex-span"><i>w</i></span>, and <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>h</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">2 ≤ <i>w</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of rows, columns, and barriers in the machine respectively.</p><p>Next <span class="tex-span"><i>n</i></span> lines describe barriers. <span class="tex-span"><i>i</i></span>-th of these lines containts four integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>, and <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub> ≤ <i>h</i></span>, <span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>w</i></span>, <span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— row index, leftmost and rightmost column index of <span class="tex-span"><i>i</i></span>-th barrier, and largest relative fall height such that the barrier does not evade a falling marble. It is guaranteed that each row has at least one free cell, and that all <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> are distinct.</p>

## Output

<p>Print one integer&nbsp;— the answer to the problem modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
10 5 1
3 2 3 10

```




```input2
10 5 2
3 1 3 10
5 3 5 10

```




```input3
10 5 2
3 1 3 7
5 3 5 10

```




```input4
10 15 4
7 3 9 5
6 4 10 1
1 1 4 10
4 11 11 20

```




```output1
7

```




```output2
16

```




```output3
14

```




```output4
53

```



## Note

<p>In the first sample case, there is a single barrier: if one throws a marble in the second or the third column, two marbles come out, otherwise there is only one. The total answer is <span class="tex-span">7</span>.</p><p>In the second sample case, the numbers of resulting marbles are <span class="tex-span">2</span>, <span class="tex-span">2</span>, <span class="tex-span">4</span>, <span class="tex-span">4</span>, <span class="tex-span">4</span> in order of indexing columns with the initial marble.</p><p>In the third sample case, the numbers of resulting marbles are <span class="tex-span">1</span>, <span class="tex-span">1</span>, <span class="tex-span">4</span>, <span class="tex-span">4</span>, <span class="tex-span">4</span>. Note that the first barrier evades the marbles falling from the top of the board, but does not evade the marbles falling from the second barrier.</p><p>In the fourth sample case, the numbers of resulting marbles are <span class="tex-span">2</span>, <span class="tex-span">2</span>, <span class="tex-span">6</span>, <span class="tex-span">6</span>, <span class="tex-span">6</span>, <span class="tex-span">6</span>, <span class="tex-span">6</span>, <span class="tex-span">6</span>, <span class="tex-span">6</span>, <span class="tex-span">1</span>, <span class="tex-span">2</span>, <span class="tex-span">1</span>, <span class="tex-span">1</span>, <span class="tex-span">1</span>, <span class="tex-span">1</span>. The picture below shows the case when a marble is thrown into the seventh column.</p><center> <img class="tex-graphics" height="529px" src="file://IE1lJMP1.png" style="max-width: 100.0%;max-height: 100.0%;" width="756px">   <span class="tex-font-size-small">The result of throwing a marble into the seventh column.</span> </center>
