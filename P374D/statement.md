## Description

<div><p>Dima's spent much time thinking what present to give to Inna and gave her an empty sequence <span class="tex-span"><i>w</i></span>. Now they want to fill sequence <span class="tex-span"><i>w</i></span> with numbers zero and one. For that, they decided to play an amusing game. </p><p>Before the game begins, Dima chooses <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>m</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index">1</sub> &lt; <i>a</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>a</i><sub class="lower-index"><i>m</i></sub>)</span>. Then Inna and Dima start playing, that is, adding numbers to sequence <span class="tex-span"><i>w</i></span>. Each new number they choose is added to the end of the sequence. At some moments of time Dima feels that the game is going to end too soon (and he wants to play with Inna as long as possible), so he hits a table hard with his fist. At that the <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>-th, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>-th, <span class="tex-span"><i>a</i><sub class="lower-index">3</sub></span>-th, <span class="tex-span">...</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>k</i></sub></span>-th numbers from the beginning simultaneously fall out of the sequence (the sequence gets <span class="tex-span"><i>k</i></span> numbers less). Here <span class="tex-span"><i>k</i></span> is such maximum number that value <span class="tex-span"><i>a</i><sub class="lower-index"><i>k</i></sub></span> doesn't exceed the current length of the sequence. If number <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span> is larger than the current length of <span class="tex-span"><i>w</i></span>, then nothing falls out of the sequence.</p><p>You are given the chronological sequence of events in the game. Each event is either adding a number to the end of sequence <span class="tex-span"><i>w</i></span> or Dima's hit on the table. Calculate the sequence <span class="tex-span"><i>w</i></span> after all these events happen.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">6</sup>)</span> showing how many events took place and how many numbers Dima chose.</p><p>The next line contains <span class="tex-span"><i>m</i></span> distinct integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup>)</span> sorted in the increasing order. </p><p>Next <span class="tex-span"><i>n</i></span> lines describe the events in the chronological order. Each line contains a single integer: -1, 0 or 1. Number -1 means that Dima hits the table. Number 0 means that Inna and Dima add number 0 to the end of the sequence. Number 1 means that Inna and Dima add number 1 to the end of the sequence.</p></div><div class="output-specification"><p>In a single line print a sequence of numbers 0 and 1 — the elements of the sequence after all events happen. Print the elements of the sequence in the order from the beginning to the end of the sequence.</p><p>If after all events the sequence ends up <span class="tex-font-style-bf">empty</span>, print "<span class="tex-font-style-tt">Poor stack!</span>".</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">6</sup>)</span> showing how many events took place and how many numbers Dima chose.</p><p>The next line contains <span class="tex-span"><i>m</i></span> distinct integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup>)</span> sorted in the increasing order. </p><p>Next <span class="tex-span"><i>n</i></span> lines describe the events in the chronological order. Each line contains a single integer: -1, 0 or 1. Number -1 means that Dima hits the table. Number 0 means that Inna and Dima add number 0 to the end of the sequence. Number 1 means that Inna and Dima add number 1 to the end of the sequence.</p>

## Output

<p>In a single line print a sequence of numbers 0 and 1 — the elements of the sequence after all events happen. Print the elements of the sequence in the order from the beginning to the end of the sequence.</p><p>If after all events the sequence ends up <span class="tex-font-style-bf">empty</span>, print "<span class="tex-font-style-tt">Poor stack!</span>".</p>





```input1
10 3
1 3 6
-1
1
1
0
0
-1
0
1
-1
1

```




```input2
2 1
1
1
-1

```




```output1
011

```




```output2
Poor stack!

```


