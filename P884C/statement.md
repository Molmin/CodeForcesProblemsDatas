## Description

<div><p>The construction of subway in Bertown is almost finished! The President of Berland will visit this city soon to look at the new subway himself.</p><p>There are <span class="tex-span"><i>n</i></span> stations in the subway. It was built according to the <span class="tex-font-style-it">Bertown Transport Law</span>:</p><ol> <li> For each station <span class="tex-span"><i>i</i></span> there exists exactly one train that goes from this station. Its destination station is <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>, possibly <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> = <i>i</i></span>; </li><li> For each station <span class="tex-span"><i>i</i></span> there exists exactly one station <span class="tex-span"><i>j</i></span> such that <span class="tex-span"><i>p</i><sub class="lower-index"><i>j</i></sub> = <i>i</i></span>. </li></ol><p>The President will consider the <span class="tex-font-style-it">convenience</span> of subway after visiting it. The <span class="tex-font-style-it">convenience</span> is the number of ordered pairs <span class="tex-span">(<i>x</i>, <i>y</i>)</span> such that person can start at station <span class="tex-span"><i>x</i></span> and, after taking some subway trains (possibly zero), arrive at station <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i></span>).</p><p>The mayor of Bertown thinks that if the subway is not <span class="tex-font-style-it">convenient</span> enough, then the President might consider installing a new mayor (and, of course, the current mayor doesn't want it to happen). Before President visits the city mayor has enough time to rebuild some paths of subway, thus changing the values of <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> for <span class="tex-font-style-bf">not more than two subway stations</span>. Of course, breaking the <span class="tex-font-style-it">Bertown Transport Law</span> is really bad, so the subway must be built according to the <span class="tex-font-style-it">Law</span> even after changes.</p><p>The mayor wants to do these changes in such a way that the <span class="tex-font-style-it">convenience</span> of the subway is maximized. Help him to calculate the maximum possible <span class="tex-font-style-it">convenience</span> he can get! </p></div><div class="input-specification"><p>The first line contains one integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100000</span>) — the number of stations.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>p</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the current structure of the subway. All these numbers are distinct.</p></div><div class="output-specification"><p>Print one number — the maximum possible value of <span class="tex-font-style-it">convenience</span>.</p></div>

## Input

<p>The first line contains one integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100000</span>) — the number of stations.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>p</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the current structure of the subway. All these numbers are distinct.</p>

## Output

<p>Print one number — the maximum possible value of <span class="tex-font-style-it">convenience</span>.</p>





```input1
3
2 1 3

```




```input2
5
1 5 4 3 2

```




```output1
9

```




```output2
17

```



## Note

<p>In the first example the mayor can change <span class="tex-span"><i>p</i><sub class="lower-index">2</sub></span> to <span class="tex-span">3</span> and <span class="tex-span"><i>p</i><sub class="lower-index">3</sub></span> to <span class="tex-span">1</span>, so there will be <span class="tex-span">9</span> pairs: <span class="tex-span">(1, 1)</span>, <span class="tex-span">(1, 2)</span>, <span class="tex-span">(1, 3)</span>, <span class="tex-span">(2, 1)</span>, <span class="tex-span">(2, 2)</span>, <span class="tex-span">(2, 3)</span>, <span class="tex-span">(3, 1)</span>, <span class="tex-span">(3, 2)</span>, <span class="tex-span">(3, 3)</span>.</p><p>In the second example the mayor can change <span class="tex-span"><i>p</i><sub class="lower-index">2</sub></span> to <span class="tex-span">4</span> and <span class="tex-span"><i>p</i><sub class="lower-index">3</sub></span> to <span class="tex-span">5</span>.</p>
