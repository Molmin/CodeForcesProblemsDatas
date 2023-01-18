## Description

<div><p>Petya and Gena love playing table tennis. A single match is played according to the following rules: a match consists of multiple sets, each set consists of multiple serves. Each serve is won by one of the players, this player scores one point. As soon as one of the players scores <span class="tex-span"><i>t</i></span> points, he wins the set; then the next set starts and scores of both players are being set to 0. As soon as one of the players wins the total of <span class="tex-span"><i>s</i></span> sets, he wins the match and the match is over. Here <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> are some positive integer numbers.</p><p>To spice it up, Petya and Gena choose new numbers <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> before every match. Besides, for the sake of history they keep a record of each match: that is, for each serve they write down the winner. Serve winners are recorded in the chronological order. In a record the set is over as soon as one of the players scores <span class="tex-span"><i>t</i></span> points and the match is over as soon as one of the players wins <span class="tex-span"><i>s</i></span> sets.</p><p>Petya and Gena have found a record of an old match. Unfortunately, the sequence of serves in the record isn't divided into sets and numbers <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> for the given match are also lost. The players now wonder what values of <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> might be. Can you determine all the possible options?</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span>&nbsp;— the length of the sequence of games (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. If <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = 1</span>, then the <span class="tex-span"><i>i</i></span>-th serve was won by Petya, if <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = 2</span>, then the <span class="tex-span"><i>i</i></span>-th serve was won by Gena.</p><p><span class="tex-font-style-bf">It is not guaranteed</span> that at least one option for numbers <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> corresponds to the given record.</p></div><div class="output-specification"><p>In the first line print a single number <span class="tex-span"><i>k</i></span>&nbsp;— the number of options for numbers <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span>.</p><p>In each of the following <span class="tex-span"><i>k</i></span> lines print two integers <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— the option for numbers <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span>. Print the options in the order of increasing <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>, and for equal <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— in the order of increasing <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span>&nbsp;— the length of the sequence of games (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. If <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = 1</span>, then the <span class="tex-span"><i>i</i></span>-th serve was won by Petya, if <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = 2</span>, then the <span class="tex-span"><i>i</i></span>-th serve was won by Gena.</p><p><span class="tex-font-style-bf">It is not guaranteed</span> that at least one option for numbers <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> corresponds to the given record.</p>

## Output

<p>In the first line print a single number <span class="tex-span"><i>k</i></span>&nbsp;— the number of options for numbers <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span>.</p><p>In each of the following <span class="tex-span"><i>k</i></span> lines print two integers <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— the option for numbers <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span>. Print the options in the order of increasing <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>, and for equal <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— in the order of increasing <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>.</p>





```input1
5
1 2 1 2 1

```




```input2
4
1 1 1 1

```




```input3
4
1 2 1 2

```




```input4
8
2 1 2 1 1 1 1 1

```




```output1
2
1 3
3 1

```




```output2
3
1 4
2 2
4 1

```




```output3
0

```




```output4
3
1 6
2 3
6 1

```


