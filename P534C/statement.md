## Description

<div><p>Polycarp has <span class="tex-span"><i>n</i></span> dice <span class="tex-span"><i>d</i><sub class="lower-index">1</sub>, <i>d</i><sub class="lower-index">2</sub>, ..., <i>d</i><sub class="lower-index"><i>n</i></sub></span>. The <span class="tex-span"><i>i</i></span>-th dice shows numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>. Polycarp rolled all the dice and the sum of numbers they showed is <span class="tex-span"><i>A</i></span>. Agrippina didn't see which dice showed what number, she knows only the sum <span class="tex-span"><i>A</i></span> and the values <span class="tex-span"><i>d</i><sub class="lower-index">1</sub>, <i>d</i><sub class="lower-index">2</sub>, ..., <i>d</i><sub class="lower-index"><i>n</i></sub></span>. However, she finds it enough to make a series of statements of the following type: dice <span class="tex-span"><i>i</i></span> couldn't show number <span class="tex-span"><i>r</i></span>. For example, if Polycarp had two six-faced dice and the total sum is <span class="tex-span"><i>A</i> = 11</span>, then Agrippina can state that each of the two dice couldn't show a value less than five (otherwise, the remaining dice must have a value of at least seven, which is impossible).</p><p>For each dice find the number of values for which it can be guaranteed that the dice couldn't show these values if the sum of the shown values is <span class="tex-span"><i>A</i></span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i>, <i>A</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup>, <i>n</i> ≤ <i>A</i> ≤ <i>s</i></span>) — the number of dice and the sum of shown values where <span class="tex-span"><i>s</i> = <i>d</i><sub class="lower-index">1</sub> + <i>d</i><sub class="lower-index">2</sub> + ... + <i>d</i><sub class="lower-index"><i>n</i></sub></span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>d</i><sub class="lower-index">1</sub>, <i>d</i><sub class="lower-index">2</sub>, ..., <i>d</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>), where <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> is the maximum value that the <span class="tex-span"><i>i</i></span>-th dice can show.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> is the number of values for which it is guaranteed that the <span class="tex-span"><i>i</i></span>-th dice couldn't show them.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i>, <i>A</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup>, <i>n</i> ≤ <i>A</i> ≤ <i>s</i></span>) — the number of dice and the sum of shown values where <span class="tex-span"><i>s</i> = <i>d</i><sub class="lower-index">1</sub> + <i>d</i><sub class="lower-index">2</sub> + ... + <i>d</i><sub class="lower-index"><i>n</i></sub></span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>d</i><sub class="lower-index">1</sub>, <i>d</i><sub class="lower-index">2</sub>, ..., <i>d</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>), where <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> is the maximum value that the <span class="tex-span"><i>i</i></span>-th dice can show.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> is the number of values for which it is guaranteed that the <span class="tex-span"><i>i</i></span>-th dice couldn't show them.</p>





```input1
2 8
4 4

```




```input2
1 3
5

```




```input3
2 3
2 3

```




```output1
3 3
```




```output2
4
```




```output3
0 1
```



## Note

<p>In the first sample from the statement <span class="tex-span"><i>A</i></span> equal to 8 could be obtained in the only case when both the first and the second dice show 4. Correspondingly, both dice couldn't show values 1, 2 or 3.</p><p>In the second sample from the statement <span class="tex-span"><i>A</i></span> equal to 3 could be obtained when the single dice shows 3. Correspondingly, it couldn't show 1, 2, 4 or 5.</p><p>In the third sample from the statement <span class="tex-span"><i>A</i></span> equal to 3 could be obtained when one dice shows 1 and the other dice shows 2. That's why the first dice doesn't have any values it couldn't show and the second dice couldn't show 3.</p>
