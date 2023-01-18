## Description

<div><p>One day Igor K. stopped programming and took up math. One late autumn evening he was sitting at a table reading a book and thinking about something. </p><p>The following statement caught his attention: "Among any six people there are either three pairwise acquainted people or three pairwise unacquainted people"</p><p>Igor just couldn't get why the required minimum is 6 people. "Well, that's the same for five people, too!" — he kept on repeating in his mind. — "Let's take, say, Max, Ilya, Vova — here, they all know each other! And now let's add Dima and Oleg to Vova — none of them is acquainted with each other! Now, that math is just rubbish!"</p><p>Igor K. took 5 friends of his and wrote down who of them is friends with whom. Now he wants to check whether it is true for the five people that among them there are either three pairwise acquainted or three pairwise not acquainted people.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(0 ≤ <i>m</i> ≤ 10)</span>, which is the number of relations of acquaintances among the five friends of Igor's.</p><p>Each of the following <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 5;<i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>)</span>, where (<span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span>) is a pair of acquainted people. It is guaranteed that each pair of the acquaintances is described exactly once. The acquaintance relation is symmetrical, i.e. if <span class="tex-span"><i>x</i></span> is acquainted with <span class="tex-span"><i>y</i></span>, then <span class="tex-span"><i>y</i></span> is also acquainted with <span class="tex-span"><i>x</i></span>.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">FAIL</span>", if among those five people there are no either three pairwise acquainted or three pairwise unacquainted people. Otherwise print "<span class="tex-font-style-tt">WIN</span>".</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(0 ≤ <i>m</i> ≤ 10)</span>, which is the number of relations of acquaintances among the five friends of Igor's.</p><p>Each of the following <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 5;<i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>)</span>, where (<span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span>) is a pair of acquainted people. It is guaranteed that each pair of the acquaintances is described exactly once. The acquaintance relation is symmetrical, i.e. if <span class="tex-span"><i>x</i></span> is acquainted with <span class="tex-span"><i>y</i></span>, then <span class="tex-span"><i>y</i></span> is also acquainted with <span class="tex-span"><i>x</i></span>.</p>

## Output

<p>Print "<span class="tex-font-style-tt">FAIL</span>", if among those five people there are no either three pairwise acquainted or three pairwise unacquainted people. Otherwise print "<span class="tex-font-style-tt">WIN</span>".</p>





```input1
4
1 3
2 3
1 4
5 3

```




```input2
5
1 2
2 3
3 4
4 5
5 1

```




```output1
WIN

```




```output2
FAIL

```


