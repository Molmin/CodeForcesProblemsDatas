## Description

<div><p>You have decided to watch the best moments of some movie. There are two buttons on your player: </p><ol> <li> Watch the current minute of the movie. By pressing this button, you watch the current minute of the movie and the player automatically proceeds to the next minute of the movie. </li><li> Skip exactly <span class="tex-span"><i>x</i></span> minutes of the movie (<span class="tex-span"><i>x</i></span> is some fixed positive integer). If the player is now at the <span class="tex-span"><i>t</i></span>-th minute of the movie, then as a result of pressing this button, it proceeds to the minute <span class="tex-span">(<i>t</i> + <i>x</i>)</span>. </li></ol><p>Initially the movie is turned on in the player on the first minute, and you want to watch exactly <span class="tex-span"><i>n</i></span> best moments of the movie, the <span class="tex-span"><i>i</i></span>-th best moment starts at the <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>-th minute and ends at the <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>-th minute (more formally, the <span class="tex-span"><i>i</i></span>-th best moment consists of minutes: <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>l</i><sub class="lower-index"><i>i</i></sub> + 1, ..., <i>r</i><sub class="lower-index"><i>i</i></sub></span>). </p><p>Determine, what is the minimum number of minutes of the movie you have to watch if you want to watch all the best moments?</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>, <span class="tex-span">1 ≤ <i>x</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of the best moments of the movie and the value of <span class="tex-span"><i>x</i></span> for the second button.</p><p>The following <span class="tex-span"><i>n</i></span> lines contain the descriptions of the best moments of the movie, the <span class="tex-span"><i>i</i></span>-th line of the description contains two integers separated by a space <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>It is guaranteed that for all integers <span class="tex-span"><i>i</i></span> from <span class="tex-span">2</span> to <span class="tex-span"><i>n</i></span> the following condition holds: <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i> - 1</sub> &lt; <i>l</i><sub class="lower-index"><i>i</i></sub></span>.</p></div><div class="output-specification"><p>Output a single number — the answer to the problem.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>, <span class="tex-span">1 ≤ <i>x</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of the best moments of the movie and the value of <span class="tex-span"><i>x</i></span> for the second button.</p><p>The following <span class="tex-span"><i>n</i></span> lines contain the descriptions of the best moments of the movie, the <span class="tex-span"><i>i</i></span>-th line of the description contains two integers separated by a space <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>It is guaranteed that for all integers <span class="tex-span"><i>i</i></span> from <span class="tex-span">2</span> to <span class="tex-span"><i>n</i></span> the following condition holds: <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i> - 1</sub> &lt; <i>l</i><sub class="lower-index"><i>i</i></sub></span>.</p>

## Output

<p>Output a single number — the answer to the problem.</p>





```input1
2 3
5 6
10 12

```




```input2
1 1
1 100000

```




```output1
6

```




```output2
100000

```



## Note

<p>In the first sample, the player was initially standing on the first minute. As the minutes from the <span class="tex-span">1</span>-st to the <span class="tex-span">4</span>-th one don't contain interesting moments, we press the second button. Now we can not press the second button and skip <span class="tex-span">3</span> more minutes, because some of them contain interesting moments. Therefore, we watch the movie from the <span class="tex-span">4</span>-th to the <span class="tex-span">6</span>-th minute, after that the current time is <span class="tex-span">7</span>. Similarly, we again skip <span class="tex-span">3</span> minutes and then watch from the <span class="tex-span">10</span>-th to the <span class="tex-span">12</span>-th minute of the movie. In total, we watch <span class="tex-span">6</span> minutes of the movie.</p><p>In the second sample, the movie is very interesting, so you'll have to watch all <span class="tex-span">100000</span> minutes of the movie.</p>
