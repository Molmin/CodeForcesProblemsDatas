## Description

<div><p>Recently Ivan bought a new computer. Excited, he unpacked it and installed his favourite game. With his old computer Ivan had to choose the worst possible graphic settings (because otherwise the framerate would be really low), but now he wants to check, maybe his new computer can perform well even with the best possible graphics?</p><p>There are <span class="tex-span"><i>m</i></span> graphics parameters in the game. <span class="tex-span"><i>i</i></span>-th parameter can be set to any positive integer from <span class="tex-span">1</span> to <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, and initially is set to <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub></span>). So there are <img align="middle" class="tex-formula" src="file://zLmsgOu4.png" style="max-width: 100.0%;max-height: 100.0%;"> different combinations of parameters. Ivan can increase or decrease any of these parameters by <span class="tex-span">1</span>; after that the game will be restarted with new parameters (and Ivan will have the opportunity to check chosen combination of parameters).</p><p>Ivan wants to try all <span class="tex-span"><i>p</i></span> possible combinations. Also he wants to return to the initial settings after trying all combinations, because he thinks that initial settings can be somehow best suited for his hardware. But Ivan doesn't really want to make a lot of restarts.</p><p>So he wants you to tell the following:</p><ul> <li> If there exists a way to make exactly <span class="tex-span"><i>p</i></span> changes (each change either decreases or increases some parameter by <span class="tex-span">1</span>) to try all possible combinations and return to initial combination, then Ivan wants to know this way. </li><li> Otherwise, if there exists a way to make exactly <span class="tex-span"><i>p</i> - 1</span> changes to try all possible combinations (including the initial one), then Ivan wants to know this way. </li></ul><p>Help Ivan by showing him the way to change parameters!</p></div><div class="input-specification"><p>The first line of input contains one integer number <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 6</span>).</p><p>The second line contains <span class="tex-span"><i>m</i></span> integer numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">2 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>). It is guaranteed that <img align="middle" class="tex-formula" src="file://sLvU8mo8.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>The third line contains <span class="tex-span"><i>m</i></span> integer numbers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub></span>).</p></div><div class="output-specification"><p>If there is a way to make exactly <span class="tex-span"><i>p</i></span> changes (each change either decreases or increases some parameter by <span class="tex-span">1</span>) to try all possible combinations and return to initial combination, then output <span class="tex-font-style-tt">Cycle</span> in the first line. Then <span class="tex-span"><i>p</i></span> lines must follow, each desribing a change. The line must be either <span class="tex-font-style-tt">inc x</span> (increase parameter <span class="tex-span"><i>x</i></span> by <span class="tex-span">1</span>) or <span class="tex-font-style-tt">dec x</span> (decrease it).</p><p>Otherwise, if there is a way to make exactly <span class="tex-span"><i>p</i> - 1</span> changes to try all possible combinations (including the initial one), then output <span class="tex-font-style-tt">Path</span> in the first line. Then <span class="tex-span"><i>p</i> - 1</span> lines must follow, each describing the change the same way as mentioned above.</p><p>Otherwise, output <span class="tex-font-style-tt">No</span>.</p></div>

## Input

<p>The first line of input contains one integer number <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 6</span>).</p><p>The second line contains <span class="tex-span"><i>m</i></span> integer numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">2 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>). It is guaranteed that <img align="middle" class="tex-formula" src="file://sLvU8mo8.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>The third line contains <span class="tex-span"><i>m</i></span> integer numbers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub></span>).</p>

## Output

<p>If there is a way to make exactly <span class="tex-span"><i>p</i></span> changes (each change either decreases or increases some parameter by <span class="tex-span">1</span>) to try all possible combinations and return to initial combination, then output <span class="tex-font-style-tt">Cycle</span> in the first line. Then <span class="tex-span"><i>p</i></span> lines must follow, each desribing a change. The line must be either <span class="tex-font-style-tt">inc x</span> (increase parameter <span class="tex-span"><i>x</i></span> by <span class="tex-span">1</span>) or <span class="tex-font-style-tt">dec x</span> (decrease it).</p><p>Otherwise, if there is a way to make exactly <span class="tex-span"><i>p</i> - 1</span> changes to try all possible combinations (including the initial one), then output <span class="tex-font-style-tt">Path</span> in the first line. Then <span class="tex-span"><i>p</i> - 1</span> lines must follow, each describing the change the same way as mentioned above.</p><p>Otherwise, output <span class="tex-font-style-tt">No</span>.</p>





```input1
1
3
1

```




```input2
1
3
2

```




```input3
2
3 2
1 1

```




```output1
Path
inc 1
inc 1

```




```output2
No

```




```output3
Cycle
inc 1
inc 1
inc 2
dec 1
dec 1
dec 2

```


