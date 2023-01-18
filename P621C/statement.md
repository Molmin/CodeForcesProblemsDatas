## Description

<div><p>There are <span class="tex-span"><i>n</i></span> sharks who grow flowers for Wet Shark. They are all sitting around the table, such that sharks <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>i</i> + 1</span> are neighbours for all <span class="tex-span"><i>i</i></span> from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i> - 1</span>. Sharks <span class="tex-span"><i>n</i></span> and <span class="tex-span">1</span> are neighbours too.</p><p>Each shark will grow some number of flowers <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>. For <span class="tex-span"><i>i</i></span>-th shark value <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> is random integer equiprobably chosen in range from <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>. Wet Shark has it's favourite prime number <span class="tex-span"><i>p</i></span>, and he really likes it! If for any pair of <span class="tex-font-style-bf">neighbouring</span> sharks <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> the product <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub>·<i>s</i><sub class="lower-index"><i>j</i></sub></span> is divisible by <span class="tex-span"><i>p</i></span>, then Wet Shark becomes happy and gives <span class="tex-span">1000</span> dollars to each of these sharks.</p><p>At the end of the day sharks sum all the money Wet Shark granted to them. Find the expectation of this value.</p></div><div class="input-specification"><p>The first line of the input contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>p</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 100 000, 2 ≤ <i>p</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of sharks and Wet Shark's favourite prime number. It is guaranteed that <span class="tex-span"><i>p</i></span> is prime.</p><p>The <span class="tex-span"><i>i</i></span>-th of the following <span class="tex-span"><i>n</i></span> lines contains information about <span class="tex-span"><i>i</i></span>-th shark&nbsp;— two space-separated integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), the range of flowers shark <span class="tex-span"><i>i</i></span> can produce. Remember that <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> is chosen equiprobably among all integers from <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>, inclusive.</p></div><div class="output-specification"><p>Print a single real number — the expected number of dollars that the sharks receive in total. You answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. </p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct, if <img align="middle" class="tex-formula" src="file://967g2U8b.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first line of the input contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>p</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 100 000, 2 ≤ <i>p</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of sharks and Wet Shark's favourite prime number. It is guaranteed that <span class="tex-span"><i>p</i></span> is prime.</p><p>The <span class="tex-span"><i>i</i></span>-th of the following <span class="tex-span"><i>n</i></span> lines contains information about <span class="tex-span"><i>i</i></span>-th shark&nbsp;— two space-separated integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), the range of flowers shark <span class="tex-span"><i>i</i></span> can produce. Remember that <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> is chosen equiprobably among all integers from <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>, inclusive.</p>

## Output

<p>Print a single real number — the expected number of dollars that the sharks receive in total. You answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. </p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct, if <img align="middle" class="tex-formula" src="file://967g2U8b.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
3 2
1 2
420 421
420420 420421

```




```input2
3 5
1 4
2 3
11 14

```




```output1
4500.0

```




```output2
0.0

```



## Note

<p>A prime number is a positive integer number that is divisible only by <span class="tex-span">1</span> and itself. <span class="tex-span">1</span> is not considered to be prime.</p><p>Consider the first sample. First shark grows some number of flowers from <span class="tex-span">1</span> to <span class="tex-span">2</span>, second sharks grows from <span class="tex-span">420</span> to <span class="tex-span">421</span> flowers and third from <span class="tex-span">420420</span> to <span class="tex-span">420421</span>. There are eight cases for the quantities of flowers <span class="tex-span">(<i>s</i><sub class="lower-index">0</sub>, <i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>)</span> each shark grows:</p><ol><li> <span class="tex-span">(1, 420, 420420)</span>: note that <span class="tex-span"><i>s</i><sub class="lower-index">0</sub>·<i>s</i><sub class="lower-index">1</sub> = 420</span>, <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>·<i>s</i><sub class="lower-index">2</sub> = 176576400</span>, and <span class="tex-span"><i>s</i><sub class="lower-index">2</sub>·<i>s</i><sub class="lower-index">0</sub> = 420420</span>. For each pair, <span class="tex-span">1000</span> dollars will be awarded to each shark. Therefore, each shark will be awarded <span class="tex-span">2000</span> dollars, for a total of <span class="tex-span">6000</span> dollars.</li><li> <span class="tex-span">(1, 420, 420421)</span>: now, the product <span class="tex-span"><i>s</i><sub class="lower-index">2</sub>·<i>s</i><sub class="lower-index">0</sub></span> is not divisible by <span class="tex-span">2</span>. Therefore, sharks <span class="tex-span"><i>s</i><sub class="lower-index">0</sub></span> and <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> will receive <span class="tex-span">1000</span> dollars, while shark <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> will receive <span class="tex-span">2000</span>. The total is <span class="tex-span">4000</span>.</li><li> <span class="tex-span">(1, 421, 420420)</span>: total is <span class="tex-span">4000</span> </li><li> <span class="tex-span">(1, 421, 420421)</span>: total is <span class="tex-span">0</span>. </li><li> <span class="tex-span">(2, 420, 420420)</span>: total is <span class="tex-span">6000</span>. </li><li> <span class="tex-span">(2, 420, 420421)</span>: total is <span class="tex-span">6000</span>. </li><li> <span class="tex-span">(2, 421, 420420)</span>: total is <span class="tex-span">6000</span>. </li><li><span class="tex-span">(2, 421, 420421)</span>: total is <span class="tex-span">4000</span>.</li></ol><p>The expected value is <img align="middle" class="tex-formula" src="file://9gRVsujb.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>In the second sample, no combination of quantities will garner the sharks any money.</p>
