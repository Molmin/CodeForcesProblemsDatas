## Description

<div><p>All cinema halls in Berland are rectangles with <span class="tex-span"><i>K</i></span> rows of <span class="tex-span"><i>K</i></span> seats each, and <span class="tex-span"><i>K</i></span> is an odd number. Rows and seats are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>K</i></span>. For safety reasons people, who come to the box office to buy tickets, are not allowed to choose seats themselves. Formerly the choice was made by a cashier, but now this is the responsibility of a special seating program. It was found out that the large majority of Berland's inhabitants go to the cinema in order to watch a movie, that's why they want to sit as close to the hall center as possible. Moreover, a company of <span class="tex-span"><i>M</i></span> people, who come to watch a movie, want necessarily to occupy <span class="tex-span"><i>M</i></span> successive seats in one row. Let's formulate the algorithm, according to which the program chooses seats and sells tickets. As the request for <span class="tex-span"><i>M</i></span> seats comes, the program should determine the row number <span class="tex-span"><i>x</i></span> and the segment <span class="tex-span">[<i>y</i><sub class="lower-index"><i>l</i></sub>, <i>y</i><sub class="lower-index"><i>r</i></sub>]</span> of the seats numbers in this row, where <span class="tex-span"><i>y</i><sub class="lower-index"><i>r</i></sub> - <i>y</i><sub class="lower-index"><i>l</i></sub> + 1 = <i>M</i></span>. From all such possible variants as a final result the program should choose the one with the minimum function value of total seats remoteness from the center. Say, <img align="middle" class="tex-formula" src="file://NPO16lHR.png" style="max-width: 100.0%;max-height: 100.0%;"> — the row and the seat numbers of the most "central" seat. Then the function value of seats remoteness from the hall center is <img align="middle" class="tex-formula" src="file://VByObvpk.png" style="max-width: 100.0%;max-height: 100.0%;">. If the amount of minimum function values is more than one, the program should choose the one that is closer to the screen (i.e. the row number <span class="tex-span"><i>x</i></span> is lower). If the variants are still multiple, it should choose the one with the minimum <span class="tex-span"><i>y</i><sub class="lower-index"><i>l</i></sub></span>. If you did not get yet, your task is to simulate the work of this program. </p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>N</i></span> and <span class="tex-span"><i>K</i></span> (<span class="tex-span">1 ≤ <i>N</i> ≤ 1000, 1 ≤ <i>K</i> ≤ 99</span>) — the amount of requests and the hall size respectively. The second line contains <span class="tex-span"><i>N</i></span> space-separated integers <span class="tex-span"><i>M</i><sub class="lower-index"><i>i</i></sub></span> from the range <span class="tex-span">[1, <i>K</i>]</span> — requests to the program.</p></div><div class="output-specification"><p>Output <span class="tex-span"><i>N</i></span> lines. In the <span class="tex-span"><i>i</i></span>-th line output «-1» (without quotes), if it is impossible to find <span class="tex-span"><i>M</i><sub class="lower-index"><i>i</i></sub></span> successive seats in one row, otherwise output three numbers <span class="tex-span"><i>x</i>, <i>y</i><sub class="lower-index"><i>l</i></sub>, <i>y</i><sub class="lower-index"><i>r</i></sub></span>. Separate the numbers with a space.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>N</i></span> and <span class="tex-span"><i>K</i></span> (<span class="tex-span">1 ≤ <i>N</i> ≤ 1000, 1 ≤ <i>K</i> ≤ 99</span>) — the amount of requests and the hall size respectively. The second line contains <span class="tex-span"><i>N</i></span> space-separated integers <span class="tex-span"><i>M</i><sub class="lower-index"><i>i</i></sub></span> from the range <span class="tex-span">[1, <i>K</i>]</span> — requests to the program.</p>

## Output

<p>Output <span class="tex-span"><i>N</i></span> lines. In the <span class="tex-span"><i>i</i></span>-th line output «-1» (without quotes), if it is impossible to find <span class="tex-span"><i>M</i><sub class="lower-index"><i>i</i></sub></span> successive seats in one row, otherwise output three numbers <span class="tex-span"><i>x</i>, <i>y</i><sub class="lower-index"><i>l</i></sub>, <i>y</i><sub class="lower-index"><i>r</i></sub></span>. Separate the numbers with a space.</p>





```input1
2 1
1 1

```




```input2
4 3
1 2 3 1

```




```output1
1 1 1
-1

```




```output2
2 2 2
1 1 2
3 1 3
2 1 1

```


