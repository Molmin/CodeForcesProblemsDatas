## Description

<div><p>You are given a sequence of balls <span class="tex-span"><i>A</i></span> by your teacher, each labeled with a lowercase Latin letter 'a'-'z'. You don't like the given sequence. You want to change it into a new sequence, <span class="tex-span"><i>B</i></span> that suits you better. So, you allow yourself four operations:</p><ul> <li> You can insert any ball with any label into the sequence at any position. </li><li> You can delete (remove) any ball from any position. </li><li> You can replace any ball with any other ball. </li><li> You can exchange (swap) two adjacent balls. </li></ul><p>Your teacher now places time constraints on each operation, meaning that an operation can only be performed in certain time. So, the first operation takes time <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, the second one takes <span class="tex-span"><i>t</i><sub class="lower-index"><i>d</i></sub></span>, the third one takes <span class="tex-span"><i>t</i><sub class="lower-index"><i>r</i></sub></span> and the fourth one takes <span class="tex-span"><i>t</i><sub class="lower-index"><i>e</i></sub></span>. Also, it is given that <span class="tex-span">2·<i>t</i><sub class="lower-index"><i>e</i></sub> ≥ <i>t</i><sub class="lower-index"><i>i</i></sub> + <i>t</i><sub class="lower-index"><i>d</i></sub></span>.</p><p>Find the minimal time to convert the sequence <span class="tex-span"><i>A</i></span> to the sequence <span class="tex-span"><i>B</i></span>.</p></div><div class="input-specification"><p>The first line contains four space-separated integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index"><i>d</i></sub>, <i>t</i><sub class="lower-index"><i>r</i></sub>, <i>t</i><sub class="lower-index"><i>e</i></sub></span> (<span class="tex-span">0 &lt; <i>t</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index"><i>d</i></sub>, <i>t</i><sub class="lower-index"><i>r</i></sub>, <i>t</i><sub class="lower-index"><i>e</i></sub> ≤ 100</span>). The following two lines contain sequences <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span> on separate lines. The length of each line is between 1 and 4000 characters inclusive.</p></div><div class="output-specification"><p>Print a single integer representing minimum time to convert <span class="tex-span"><i>A</i></span> into <span class="tex-span"><i>B</i></span>.</p></div>

## Input

<p>The first line contains four space-separated integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index"><i>d</i></sub>, <i>t</i><sub class="lower-index"><i>r</i></sub>, <i>t</i><sub class="lower-index"><i>e</i></sub></span> (<span class="tex-span">0 &lt; <i>t</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index"><i>d</i></sub>, <i>t</i><sub class="lower-index"><i>r</i></sub>, <i>t</i><sub class="lower-index"><i>e</i></sub> ≤ 100</span>). The following two lines contain sequences <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span> on separate lines. The length of each line is between 1 and 4000 characters inclusive.</p>

## Output

<p>Print a single integer representing minimum time to convert <span class="tex-span"><i>A</i></span> into <span class="tex-span"><i>B</i></span>.</p>





```input1
1 1 1 1
youshouldnot
thoushaltnot

```




```input2
2 4 10 3
ab
ba

```




```input3
1 10 20 30
a
za

```




```output1
5

```




```output2
3

```




```output3
1

```



## Note

<p>In the second sample, you could delete the ball labeled 'a' from the first position and then insert another 'a' at the new second position with total time 6. However exchanging the balls give total time 3.</p>
