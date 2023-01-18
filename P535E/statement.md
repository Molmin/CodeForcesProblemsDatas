## Description

<div><p><span class="tex-font-style-underline">Tavas is a cheerleader in the new sports competition named "Pashmaks".</span></p><center> <img class="tex-graphics" src="file://uEhORGcz.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>This competition consists of two part: swimming and then running. People will immediately start running <span class="tex-span"><i>R</i></span> meters after they finished swimming exactly <span class="tex-span"><i>S</i></span> meters. A winner is a such person that nobody else finishes running before him/her (there may be more than one winner).</p><p>Before the match starts, Tavas knows that there are <span class="tex-span"><i>n</i></span> competitors registered for the match. Also, he knows that <span class="tex-span"><i>i</i></span>-th person's swimming speed is <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> meters per second and his/her running speed is <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> meters per second. Unfortunately, he doesn't know the values of <span class="tex-span"><i>R</i></span> and <span class="tex-span"><i>S</i></span>, but he knows that they are real numbers greater than <span class="tex-span">0</span>.</p><p>As a cheerleader, Tavas wants to know who to cheer up. So, he wants to know all people that might win. We consider a competitor might win if and only if there are some values of <span class="tex-span"><i>R</i></span> and <span class="tex-span"><i>S</i></span> such that with these values, (s)he will be a winner.</p><p>Tavas isn't really familiar with programming, so he asked you to help him.</p></div><div class="input-specification"><p>The first line of input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2 × 10<sup class="upper-index">5</sup></span>).</p><p>The next <span class="tex-span"><i>n</i></span> lines contain the details of competitors. <span class="tex-span"><i>i</i></span>-th line contains two integers <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>).</p></div><div class="output-specification"><p>In the first and the only line of output, print a sequence of numbers of possible winners in increasing order.</p></div>

## Input

<p>The first line of input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2 × 10<sup class="upper-index">5</sup></span>).</p><p>The next <span class="tex-span"><i>n</i></span> lines contain the details of competitors. <span class="tex-span"><i>i</i></span>-th line contains two integers <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>).</p>

## Output

<p>In the first and the only line of output, print a sequence of numbers of possible winners in increasing order.</p>





```input1
3
1 3
2 2
3 1

```




```input2
3
1 2
1 1
2 1

```




```output1
1 2 3 

```




```output2
1 3 

```


