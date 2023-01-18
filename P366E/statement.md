## Description

<div><p>Dima loves Inna very much. He decided to write a song for her. Dima has a magic guitar with <span class="tex-span"><i>n</i></span> strings and <span class="tex-span"><i>m</i></span> frets. Dima makes the guitar produce sounds like that: to play a note, he needs to hold one of the strings on one of the frets and then pull the string. When Dima pulls the <span class="tex-span"><i>i</i></span>-th string holding it on the <span class="tex-span"><i>j</i></span>-th fret the guitar produces a note, let's denote it as <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span>. We know that Dima's guitar can produce <span class="tex-span"><i>k</i></span> distinct notes. It is possible that some notes can be produced in multiple ways. In other words, it is possible that <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub> = <i>a</i><sub class="lower-index"><i>pq</i></sub></span> at <span class="tex-span">(<i>i</i>, <i>j</i>) ≠ (<i>p</i>, <i>q</i>)</span>.</p><p>Dima has already written a song — a sequence of <span class="tex-span"><i>s</i></span> notes. In order to play the song, you need to consecutively produce the notes from the song on the guitar. You can produce each note in any available way. Dima understood that there are many ways to play a song and he wants to play it so as to make the song look as complicated as possible (try to act like Cobein).</p><p>We'll represent a way to play a song as a sequence of pairs <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>s</i>)</span>, such that the <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>-th string on the <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>-th fret produces the <span class="tex-span"><i>i</i></span>-th note from the song. The complexity of moving between pairs <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span> and <span class="tex-span">(<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>)</span> equals <img align="middle" class="tex-formula" src="file://kGiesBbe.png" style="max-width: 100.0%;max-height: 100.0%;"> + <img align="middle" class="tex-formula" src="file://S25FPZmv.png" style="max-width: 100.0%;max-height: 100.0%;">. The complexity of a way to play a song is the maximum of complexities of moving between adjacent pairs.</p><p>Help Dima determine the maximum complexity of the way to play his song! The guy's gotta look cool!</p></div><div class="input-specification"><p>The first line of the input contains four integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>s</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 2000, 1 ≤ <i>k</i> ≤ 9, 2 ≤ <i>s</i> ≤ 10<sup class="upper-index">5</sup>)</span>. </p><p>Then follow <span class="tex-span"><i>n</i></span> lines, each containing <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>ij</i></sub> ≤ <i>k</i>)</span>. The number in the <span class="tex-span"><i>i</i></span>-th row and the <span class="tex-span"><i>j</i></span>-th column (<span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span>) means a note that the guitar produces on the <span class="tex-span"><i>i</i></span>-th string and the <span class="tex-span"><i>j</i></span>-th fret.</p><p>The last line of the input contains <span class="tex-span"><i>s</i></span> integers <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>q</i><sub class="lower-index"><i>i</i></sub> ≤ <i>k</i>)</span> — the sequence of notes of the song.</p></div><div class="output-specification"><p>In a single line print a single number — the maximum possible complexity of the song.</p></div>

## Input

<p>The first line of the input contains four integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>s</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 2000, 1 ≤ <i>k</i> ≤ 9, 2 ≤ <i>s</i> ≤ 10<sup class="upper-index">5</sup>)</span>. </p><p>Then follow <span class="tex-span"><i>n</i></span> lines, each containing <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>ij</i></sub> ≤ <i>k</i>)</span>. The number in the <span class="tex-span"><i>i</i></span>-th row and the <span class="tex-span"><i>j</i></span>-th column (<span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span>) means a note that the guitar produces on the <span class="tex-span"><i>i</i></span>-th string and the <span class="tex-span"><i>j</i></span>-th fret.</p><p>The last line of the input contains <span class="tex-span"><i>s</i></span> integers <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>q</i><sub class="lower-index"><i>i</i></sub> ≤ <i>k</i>)</span> — the sequence of notes of the song.</p>

## Output

<p>In a single line print a single number — the maximum possible complexity of the song.</p>





```input1
4 6 5 7
3 1 2 2 3 1
3 2 2 2 5 5
4 2 2 2 5 3
3 2 2 1 4 3
2 3 1 4 1 5 1

```




```input2
4 4 9 5
4 7 9 5
1 2 1 7
8 3 4 9
5 7 7 2
7 1 9 2 5

```




```output1
8

```




```output2
4

```


