## Description

<div><p>All modern mobile applications are divided into free and paid. Even a single application developers often release two versions: a paid version without ads and a free version with ads.</p><center> <img class="tex-graphics" src="file://G1BRCrBJ.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Suppose that a paid version of the app costs <span class="tex-span"><i>p</i></span> (<span class="tex-span"><i>p</i></span> is an integer) rubles, and the free version of the application contains <span class="tex-span"><i>c</i></span> ad banners. Each user can be described by two integers: <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> — the number of rubles this user is willing to pay for the paid version of the application, and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> — the number of banners he is willing to tolerate in the free version.</p><p>The behavior of each member shall be considered strictly deterministic:</p><ul> <li> if for user <span class="tex-span"><i>i</i></span>, value <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> is at least <span class="tex-span"><i>c</i></span>, then he uses the free version, </li><li> otherwise, if value <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is at least <span class="tex-span"><i>p</i></span>, then he buys the paid version without advertising, </li><li> otherwise the user simply does not use the application. </li></ul><p>Each user of the free version brings the profit of <span class="tex-span"><i>c</i> × <i>w</i></span> rubles. Each user of the paid version brings the profit of <span class="tex-span"><i>p</i></span> rubles.</p><p>Your task is to help the application developers to select the optimal parameters <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>c</i></span>. Namely, knowing all the characteristics of users, for each value of <span class="tex-span"><i>c</i></span> from <span class="tex-span">0</span> to <span class="tex-span">(<i>max</i>&nbsp;<i>b</i><sub class="lower-index"><i>i</i></sub>) + 1</span> you need to determine the maximum profit from the application and the corresponding parameter <span class="tex-span"><i>p</i></span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>w</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;1 ≤ <i>w</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of users and the profit from a single banner. Each of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span> — the characteristics of the <span class="tex-span"><i>i</i></span>-th user.</p></div><div class="output-specification"><p>Print <span class="tex-span">(<i>max</i>&nbsp;<i>b</i><sub class="lower-index"><i>i</i></sub>) + 2</span> lines, in the <span class="tex-span"><i>i</i></span>-th line print two integers: <span class="tex-span"><i>pay</i></span> — the maximum gained profit at <span class="tex-span"><i>c</i> = <i>i</i> - 1</span>, <span class="tex-span"><i>p</i></span> <span class="tex-span">(0 ≤ <i>p</i> ≤ 10<sup class="upper-index">9</sup>)</span> — the corresponding optimal app cost. If there are multiple optimal solutions, print any of them.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>w</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;1 ≤ <i>w</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of users and the profit from a single banner. Each of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span> — the characteristics of the <span class="tex-span"><i>i</i></span>-th user.</p>

## Output

<p>Print <span class="tex-span">(<i>max</i>&nbsp;<i>b</i><sub class="lower-index"><i>i</i></sub>) + 2</span> lines, in the <span class="tex-span"><i>i</i></span>-th line print two integers: <span class="tex-span"><i>pay</i></span> — the maximum gained profit at <span class="tex-span"><i>c</i> = <i>i</i> - 1</span>, <span class="tex-span"><i>p</i></span> <span class="tex-span">(0 ≤ <i>p</i> ≤ 10<sup class="upper-index">9</sup>)</span> — the corresponding optimal app cost. If there are multiple optimal solutions, print any of them.</p>





```input1
2 1
2 0
0 2

```




```input2
3 1
3 1
2 2
1 3

```




```output1
0 3
3 2
4 2
2 2

```




```output2
0 4
3 4
7 3
7 2
4 2

```


