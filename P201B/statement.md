## Description

<div><p>A widely known among some people Belarusian sport programmer Yura possesses lots of information about cars. That is why he has been invited to participate in a game show called "Guess That Car!".</p><p>The game show takes place on a giant parking lot, which is <span class="tex-span">4<i>n</i></span> meters long from north to south and <span class="tex-span">4<i>m</i></span> meters wide from west to east. The lot has <span class="tex-span"><i>n</i> + 1</span> dividing lines drawn from west to east and <span class="tex-span"><i>m</i> + 1</span> dividing lines drawn from north to south, which divide the parking lot into <span class="tex-span"><i>n</i>·<i>m</i></span> <span class="tex-span">4</span> by <span class="tex-span">4</span> meter squares. There is a car parked strictly inside each square. The dividing lines are numbered from <span class="tex-span">0</span> to <span class="tex-span"><i>n</i></span> from north to south and from <span class="tex-span">0</span> to <span class="tex-span"><i>m</i></span> from west to east. Each square has coordinates <span class="tex-span">(<i>i</i>, <i>j</i>)</span> so that the square in the north-west corner has coordinates <span class="tex-span">(1, 1)</span> and the square in the south-east corner has coordinates <span class="tex-span">(<i>n</i>, <i>m</i>)</span>. See the picture in the notes for clarifications.</p><p>Before the game show the organizers offer Yura to occupy any of the <span class="tex-span">(<i>n</i> + 1)·(<i>m</i> + 1)</span> intersection points of the dividing lines. After that he can start guessing the cars. After Yura chooses a point, he will be prohibited to move along the parking lot before the end of the game show. As Yura is a car expert, he will always guess all cars he is offered, it's just a matter of time. Yura knows that to guess each car he needs to spend time equal to the square of the euclidean distance between his point and the center of the square with this car, multiplied by some coefficient characterizing the machine's "rarity" (the rarer the car is, the harder it is to guess it). More formally, guessing a car with "rarity" <span class="tex-span"><i>c</i></span> placed in a square whose center is at distance <span class="tex-span"><i>d</i></span> from Yura takes <span class="tex-span"><i>c</i>·<i>d</i><sup class="upper-index">2</sup></span> seconds. The time Yura spends on turning his head can be neglected.</p><p>It just so happened that Yura knows the "rarity" of each car on the parking lot in advance. Help him choose his point so that the total time of guessing all cars is the smallest possible.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 1000)</span> — the sizes of the parking lot. Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> integers: the <span class="tex-span"><i>j</i></span>-th number in the <span class="tex-span"><i>i</i></span>-th line describes the "rarity" <span class="tex-span"><i>c</i><sub class="lower-index"><i>ij</i></sub></span> (<span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>ij</i></sub> ≤ 100000</span>) of the car that is located in the square with coordinates <span class="tex-span">(<i>i</i>, <i>j</i>)</span>.</p></div><div class="output-specification"><p>In the first line print the minimum total time Yura needs to guess all offered cars. In the second line print two numbers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>l</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">0 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 0 ≤ <i>l</i><sub class="lower-index"><i>j</i></sub> ≤ <i>m</i></span>) — the numbers of dividing lines that form a junction that Yura should choose to stand on at the beginning of the game show. If there are multiple optimal starting points, print the point with smaller <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>. If there are still multiple such points, print the point with smaller <span class="tex-span"><i>l</i><sub class="lower-index"><i>j</i></sub></span>.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 1000)</span> — the sizes of the parking lot. Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> integers: the <span class="tex-span"><i>j</i></span>-th number in the <span class="tex-span"><i>i</i></span>-th line describes the "rarity" <span class="tex-span"><i>c</i><sub class="lower-index"><i>ij</i></sub></span> (<span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>ij</i></sub> ≤ 100000</span>) of the car that is located in the square with coordinates <span class="tex-span">(<i>i</i>, <i>j</i>)</span>.</p>

## Output

<p>In the first line print the minimum total time Yura needs to guess all offered cars. In the second line print two numbers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>l</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">0 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 0 ≤ <i>l</i><sub class="lower-index"><i>j</i></sub> ≤ <i>m</i></span>) — the numbers of dividing lines that form a junction that Yura should choose to stand on at the beginning of the game show. If there are multiple optimal starting points, print the point with smaller <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>. If there are still multiple such points, print the point with smaller <span class="tex-span"><i>l</i><sub class="lower-index"><i>j</i></sub></span>.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
2 3
3 4 5
3 9 1

```




```input2
3 4
1 0 0 0
0 0 3 0
0 0 5 5

```




```output1
392
1 1

```




```output2
240
2 3

```



## Note

<p>In the first test case the total time of guessing all cars is equal to 3·8 + 3·8 + 4·8 + 9·8 + 5·40 + 1·40 = 392.</p><p>The coordinate system of the field: </p><center> <img class="tex-graphics" src="file://bEc3rJMY.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
