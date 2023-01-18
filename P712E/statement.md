## Description

<div><p>There are <span class="tex-span"><i>n</i></span> casinos lined in a row. If Memory plays at casino <span class="tex-span"><i>i</i></span>, he has probability <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> to win and move to the casino on the right (<span class="tex-span"><i>i</i> + 1</span>) or exit the row (if <span class="tex-span"><i>i</i> = <i>n</i></span>), and a probability <span class="tex-span">1 - <i>p</i><sub class="lower-index"><i>i</i></sub></span> to lose and move to the casino on the left (<span class="tex-span"><i>i</i> - 1</span>) or also exit the row (if <span class="tex-span"><i>i</i> = 1</span>). </p><p>We say that Memory <span class="tex-font-style-it">dominates</span> on the interval <span class="tex-span"><i>i</i>... <i>j</i></span> if he completes a walk such that,</p><ul> <li> He starts on casino <span class="tex-span"><i>i</i></span>. </li><li> He never looses in casino <span class="tex-span"><i>i</i></span>. </li><li> He finishes his walk by winning in casino <span class="tex-span"><i>j</i></span>. </li></ul><p>Note that Memory can still walk left of the <span class="tex-span">1</span>-st casino and right of the casino <span class="tex-span"><i>n</i></span> and that always finishes the process.</p><p>Now Memory has some requests, in one of the following forms:</p><ul> <li> <span class="tex-span">1</span> <span class="tex-span"><i>i</i></span> <span class="tex-span"><i>a</i></span> <span class="tex-span"><i>b</i></span>: Set <img align="middle" class="tex-formula" src="file://5rYCd4Hu.png" style="max-width: 100.0%;max-height: 100.0%;">. </li><li> <span class="tex-span">2</span> <span class="tex-span"><i>l</i></span> <span class="tex-span"><i>r</i></span>: Print the probability that Memory will <span class="tex-font-style-it">dominate</span> on the interval <span class="tex-span"><i>l</i>... <i>r</i></span>, i.e. compute the probability that Memory will first leave the segment <span class="tex-span"><i>l</i>... <i>r</i></span> after winning at casino <span class="tex-span"><i>r</i></span>, if she starts in casino <span class="tex-span"><i>l</i></span>. </li></ul><p>It is guaranteed that at any moment of time <span class="tex-span"><i>p</i></span> is a <span class="tex-font-style-bf">non-decreasing sequence</span>, i.e. <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>p</i><sub class="lower-index"><i>i</i> + 1</sub></span> for all <span class="tex-span"><i>i</i></span> from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i> - 1</span>.</p><p>Please help Memory by answering all his requests!</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span>(<span class="tex-span">1 ≤ <i>n</i>, <i>q</i> ≤ 100 000</span>), &nbsp;— number of casinos and number of requests respectively.</p><p>The next <span class="tex-span"><i>n</i></span> lines each contain integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) &nbsp;— <img align="middle" class="tex-formula" src="file://tG8dG0os.png" style="max-width: 100.0%;max-height: 100.0%;"> is the probability <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> of winning in casino <span class="tex-span"><i>i</i></span>.</p><p>The next <span class="tex-span"><i>q</i></span> lines each contain queries of one of the types specified above (<span class="tex-span">1 ≤ <i>a</i> &lt; <i>b</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>).</p><p>It's guaranteed that there will be at least one query of type <span class="tex-span">2</span>, i.e. the output will be non-empty. Additionally, it is guaranteed that <span class="tex-span"><i>p</i></span> forms a non-decreasing sequence at all times.</p></div><div class="output-specification"><p>Print a real number for every request of type <span class="tex-span">2</span>&nbsp;— the probability that boy will "dominate" on that interval. Your answer will be considered correct if its absolute error does not exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p><p>Namely: let's assume that one of your answers is <span class="tex-span"><i>a</i></span>, and the corresponding answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct if <span class="tex-span">|<i>a</i> - <i>b</i>| ≤ 10<sup class="upper-index"> - 4</sup></span>.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span>(<span class="tex-span">1 ≤ <i>n</i>, <i>q</i> ≤ 100 000</span>), &nbsp;— number of casinos and number of requests respectively.</p><p>The next <span class="tex-span"><i>n</i></span> lines each contain integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) &nbsp;— <img align="middle" class="tex-formula" src="file://tG8dG0os.png" style="max-width: 100.0%;max-height: 100.0%;"> is the probability <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> of winning in casino <span class="tex-span"><i>i</i></span>.</p><p>The next <span class="tex-span"><i>q</i></span> lines each contain queries of one of the types specified above (<span class="tex-span">1 ≤ <i>a</i> &lt; <i>b</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>).</p><p>It's guaranteed that there will be at least one query of type <span class="tex-span">2</span>, i.e. the output will be non-empty. Additionally, it is guaranteed that <span class="tex-span"><i>p</i></span> forms a non-decreasing sequence at all times.</p>

## Output

<p>Print a real number for every request of type <span class="tex-span">2</span>&nbsp;— the probability that boy will "dominate" on that interval. Your answer will be considered correct if its absolute error does not exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p><p>Namely: let's assume that one of your answers is <span class="tex-span"><i>a</i></span>, and the corresponding answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct if <span class="tex-span">|<i>a</i> - <i>b</i>| ≤ 10<sup class="upper-index"> - 4</sup></span>.</p>





```input1
3 13
1 3
1 2
2 3
2 1 1
2 1 2
2 1 3
2 2 2
2 2 3
2 3 3
1 2 2 3
2 1 1
2 1 2
2 1 3
2 2 2
2 2 3
2 3 3

```




```output1
0.3333333333
0.2000000000
0.1666666667
0.5000000000
0.4000000000
0.6666666667
0.3333333333
0.2500000000
0.2222222222
0.6666666667
0.5714285714
0.6666666667

```


