## Description

<div><p>One day Polycarp decided to rewatch his absolute favourite episode of well-known TV series "Tufurama". He was pretty surprised when he got results only for season 7 episode 3 with his search query of "Watch Tufurama season 3 episode 7 online full hd free". This got Polycarp confused — what if he decides to rewatch the entire series someday and won't be able to find the right episodes to watch? Polycarp now wants to count the number of times he will be forced to search for an episode using some different method.</p><p>TV series have <span class="tex-span"><i>n</i></span> seasons (numbered <span class="tex-span">1</span> through <span class="tex-span"><i>n</i></span>), the <span class="tex-span"><i>i</i></span>-th season has <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> episodes (numbered <span class="tex-span">1</span> through <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>). Polycarp thinks that if for some pair of integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span"><i>x</i> &lt; <i>y</i></span>) exist both season <span class="tex-span"><i>x</i></span> episode <span class="tex-span"><i>y</i></span> and season <span class="tex-span"><i>y</i></span> episode <span class="tex-span"><i>x</i></span> then one of these search queries will include the wrong results. Help Polycarp to calculate the number of such pairs!</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1  ≤ <i>n</i>  ≤  2·10<sup class="upper-index">5</sup>)</span> — the number of seasons.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers separated by space <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> — number of episodes in each season.</p></div><div class="output-specification"><p>Print one integer — the number of pairs <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span"><i>x</i> &lt; <i>y</i></span>) such that there exist both season <span class="tex-span"><i>x</i></span> episode <span class="tex-span"><i>y</i></span> and season <span class="tex-span"><i>y</i></span> episode <span class="tex-span"><i>x</i></span>.</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1  ≤ <i>n</i>  ≤  2·10<sup class="upper-index">5</sup>)</span> — the number of seasons.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers separated by space <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> — number of episodes in each season.</p>

## Output

<p>Print one integer — the number of pairs <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span"><i>x</i> &lt; <i>y</i></span>) such that there exist both season <span class="tex-span"><i>x</i></span> episode <span class="tex-span"><i>y</i></span> and season <span class="tex-span"><i>y</i></span> episode <span class="tex-span"><i>x</i></span>.</p>





```input1
5
1 2 3 4 5

```




```input2
3
8 12 7

```




```input3
3
3 2 1

```




```output1
0

```




```output2
3

```




```output3
2

```



## Note

<p>Possible pairs in the second example:</p><ol> <li> <span class="tex-span"><i>x</i> = 1</span>, <span class="tex-span"><i>y</i> = 2</span> (season 1 episode 2 <img align="middle" class="tex-formula" src="file://EPvqZ1r8.png" style="max-width: 100.0%;max-height: 100.0%;"> season 2 episode 1); </li><li> <span class="tex-span"><i>x</i> = 2</span>, <span class="tex-span"><i>y</i> = 3</span> (season 2 episode 3 <img align="middle" class="tex-formula" src="file://C1WzurPM.png" style="max-width: 100.0%;max-height: 100.0%;"> season 3 episode 2); </li><li> <span class="tex-span"><i>x</i> = 1</span>, <span class="tex-span"><i>y</i> = 3</span> (season 1 episode 3 <img align="middle" class="tex-formula" src="file://lgy3EXv6.png" style="max-width: 100.0%;max-height: 100.0%;"> season 3 episode 1). </li></ol><p>In the third example:</p><ol> <li> <span class="tex-span"><i>x</i> = 1</span>, <span class="tex-span"><i>y</i> = 2</span> (season 1 episode 2 <img align="middle" class="tex-formula" src="file://Q3USB7q8.png" style="max-width: 100.0%;max-height: 100.0%;"> season 2 episode 1); </li><li> <span class="tex-span"><i>x</i> = 1</span>, <span class="tex-span"><i>y</i> = 3</span> (season 1 episode 3 <img align="middle" class="tex-formula" src="file://YuQW6aik.png" style="max-width: 100.0%;max-height: 100.0%;"> season 3 episode 1). </li></ol>
