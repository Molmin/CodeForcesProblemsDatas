## Description

<div><p>Nadeko's birthday is approaching! As she decorated the room for the party, a long garland of Dianthus-shaped paper pieces was placed on a prominent part of the wall. Brother Koyomi will like it!</p><p>Still unsatisfied with the garland, Nadeko decided to polish it again. The garland has <span class="tex-span"><i>n</i></span> pieces numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from left to right, and the <span class="tex-span"><i>i</i></span>-th piece has a colour <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>, denoted by a lowercase English letter. Nadeko will repaint <span class="tex-font-style-bf">at most</span> <span class="tex-span"><i>m</i></span> of the pieces to give each of them an arbitrary new colour (still denoted by a lowercase English letter). After this work, she finds out all subsegments of the garland containing pieces of only colour <span class="tex-span"><i>c</i></span> — Brother Koyomi's favourite one, and takes the length of the longest among them to be the <span class="tex-font-style-underline">Koyomity</span> of the garland.</p><p>For instance, let's say the garland is represented by "<span class="tex-font-style-tt">kooomo</span>", and Brother Koyomi's favourite colour is "<span class="tex-font-style-tt">o</span>". Among all subsegments containing pieces of "<span class="tex-font-style-tt">o</span>" only, "<span class="tex-font-style-tt">ooo</span>" is the longest, with a length of <span class="tex-span">3</span>. Thus the <span class="tex-font-style-underline">Koyomity</span> of this garland equals <span class="tex-span">3</span>.</p><p>But problem arises as Nadeko is unsure about Brother Koyomi's favourite colour, and has swaying ideas on the amount of work to do. She has <span class="tex-span"><i>q</i></span> plans on this, each of which can be expressed as a pair of an integer <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> and a lowercase letter <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>, meanings of which are explained above. You are to find out the maximum <span class="tex-font-style-underline">Koyomity</span> achievable after repainting the garland according to each plan.</p></div><div class="input-specification"><p>The first line of input contains a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1 500</span>) — the length of the garland.</p><p>The second line contains <span class="tex-span"><i>n</i></span> lowercase English letters <span class="tex-span"><i>s</i><sub class="lower-index">1</sub><i>s</i><sub class="lower-index">2</sub>... <i>s</i><sub class="lower-index"><i>n</i></sub></span> as a string — the initial colours of paper pieces on the garland.</p><p>The third line contains a positive integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 200 000</span>) — the number of plans Nadeko has.</p><p>The next <span class="tex-span"><i>q</i></span> lines describe one plan each: the <span class="tex-span"><i>i</i></span>-th among them contains an integer <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>m</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the maximum amount of pieces to repaint, followed by a space, then by a lowercase English letter <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> — Koyomi's possible favourite colour.</p></div><div class="output-specification"><p>Output <span class="tex-span"><i>q</i></span> lines: for each work plan, output one line containing an integer — the largest <span class="tex-font-style-underline">Koyomity</span> achievable after repainting the garland according to it.</p></div>

## Input

<p>The first line of input contains a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1 500</span>) — the length of the garland.</p><p>The second line contains <span class="tex-span"><i>n</i></span> lowercase English letters <span class="tex-span"><i>s</i><sub class="lower-index">1</sub><i>s</i><sub class="lower-index">2</sub>... <i>s</i><sub class="lower-index"><i>n</i></sub></span> as a string — the initial colours of paper pieces on the garland.</p><p>The third line contains a positive integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 200 000</span>) — the number of plans Nadeko has.</p><p>The next <span class="tex-span"><i>q</i></span> lines describe one plan each: the <span class="tex-span"><i>i</i></span>-th among them contains an integer <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>m</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the maximum amount of pieces to repaint, followed by a space, then by a lowercase English letter <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> — Koyomi's possible favourite colour.</p>

## Output

<p>Output <span class="tex-span"><i>q</i></span> lines: for each work plan, output one line containing an integer — the largest <span class="tex-font-style-underline">Koyomity</span> achievable after repainting the garland according to it.</p>





```input1
6
koyomi
3
1 o
4 o
4 m

```




```input2
15
yamatonadeshiko
10
1 a
2 a
3 a
4 a
5 a
1 b
2 b
3 b
4 b
5 b

```




```input3
10
aaaaaaaaaa
2
10 b
10 z

```




```output1
3
6
5

```




```output2
3
4
5
7
8
1
2
3
4
5

```




```output3
10
10

```



## Note

<p>In the first sample, there are three plans: </p><ul> <li> In the first plan, at most <span class="tex-span">1</span> piece can be repainted. Repainting the "<span class="tex-font-style-tt">y</span>" piece to become "<span class="tex-font-style-tt">o</span>" results in "<span class="tex-font-style-tt">kooomi</span>", whose <span class="tex-font-style-underline">Koyomity</span> of <span class="tex-span">3</span> is the best achievable; </li><li> In the second plan, at most <span class="tex-span">4</span> pieces can be repainted, and "<span class="tex-font-style-tt">oooooo</span>" results in a <span class="tex-font-style-underline">Koyomity</span> of <span class="tex-span">6</span>; </li><li> In the third plan, at most <span class="tex-span">4</span> pieces can be repainted, and "<span class="tex-font-style-tt">mmmmmi</span>" and "<span class="tex-font-style-tt">kmmmmm</span>" both result in a <span class="tex-font-style-underline">Koyomity</span> of <span class="tex-span">5</span>. </li></ul>
