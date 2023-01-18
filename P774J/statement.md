## Description

<div><p>Well, the series which Stepan watched for a very long time, ended. In total, the series had <span class="tex-span"><i>n</i></span> episodes. For each of them, Stepan remembers either that he definitely has watched it, or that he definitely hasn't watched it, or he is unsure, has he watched this episode or not. </p><p>Stepan's dissatisfaction is the <span class="tex-font-style-bf">maximum</span> number of consecutive series that Stepan did not watch.</p><p>Your task is to determine according to Stepan's memories if his dissatisfaction could be exactly equal to <span class="tex-span"><i>k</i></span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">0 ≤ <i>k</i> ≤ <i>n</i></span>) — the number of episodes in the series and the dissatisfaction which should be checked. </p><p>The second line contains the sequence which consists of <span class="tex-span"><i>n</i></span> symbols "<span class="tex-font-style-tt">Y</span>", "<span class="tex-font-style-tt">N</span>" and "<span class="tex-font-style-tt">?</span>". If the <span class="tex-span"><i>i</i></span>-th symbol equals "<span class="tex-font-style-tt">Y</span>", Stepan remembers that he has watched the episode number <span class="tex-span"><i>i</i></span>. If the <span class="tex-span"><i>i</i></span>-th symbol equals "<span class="tex-font-style-tt">N</span>", Stepan remembers that he hasn't watched the epizode number <span class="tex-span"><i>i</i></span>. If the <span class="tex-span"><i>i</i></span>-th symbol equals "<span class="tex-font-style-tt">?</span>", Stepan doesn't exactly remember if he has watched the episode number <span class="tex-span"><i>i</i></span> or not.</p></div><div class="output-specification"><p>If Stepan's dissatisfaction can be exactly equal to <span class="tex-span"><i>k</i></span>, then print "<span class="tex-font-style-tt">YES</span>" (without qoutes). Otherwise print "<span class="tex-font-style-tt">NO</span>" (without qoutes).</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">0 ≤ <i>k</i> ≤ <i>n</i></span>) — the number of episodes in the series and the dissatisfaction which should be checked. </p><p>The second line contains the sequence which consists of <span class="tex-span"><i>n</i></span> symbols "<span class="tex-font-style-tt">Y</span>", "<span class="tex-font-style-tt">N</span>" and "<span class="tex-font-style-tt">?</span>". If the <span class="tex-span"><i>i</i></span>-th symbol equals "<span class="tex-font-style-tt">Y</span>", Stepan remembers that he has watched the episode number <span class="tex-span"><i>i</i></span>. If the <span class="tex-span"><i>i</i></span>-th symbol equals "<span class="tex-font-style-tt">N</span>", Stepan remembers that he hasn't watched the epizode number <span class="tex-span"><i>i</i></span>. If the <span class="tex-span"><i>i</i></span>-th symbol equals "<span class="tex-font-style-tt">?</span>", Stepan doesn't exactly remember if he has watched the episode number <span class="tex-span"><i>i</i></span> or not.</p>

## Output

<p>If Stepan's dissatisfaction can be exactly equal to <span class="tex-span"><i>k</i></span>, then print "<span class="tex-font-style-tt">YES</span>" (without qoutes). Otherwise print "<span class="tex-font-style-tt">NO</span>" (without qoutes).</p>





```input1
5 2
NYNNY

```




```input2
6 1
????NN

```




```output1
YES

```




```output2
NO

```



## Note

<p>In the first test Stepan remembers about all the episodes whether he has watched them or not. His dissatisfaction is <span class="tex-span">2</span>, because he hasn't watch two episodes in a row — the episode number <span class="tex-span">3</span> and the episode number <span class="tex-span">4</span>. The answer is "<span class="tex-font-style-tt">YES</span>", because <span class="tex-span"><i>k</i> = 2</span>.</p><p>In the second test <span class="tex-span"><i>k</i> = 1</span>, Stepan's dissatisfaction is greater than or equal to <span class="tex-span">2</span> (because he remembers that he hasn't watch at least two episodes in a row — number <span class="tex-span">5</span> and number <span class="tex-span">6</span>), even if he has watched the episodes from the first to the fourth, inclusive.</p>
