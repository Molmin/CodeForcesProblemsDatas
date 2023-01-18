## Description

<div><p>Zane the wizard is going to perform a magic show shuffling the cups.</p><p>There are <span class="tex-span"><i>n</i></span> cups, numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, placed along the <span class="tex-span"><i>x</i></span>-axis on a table that has <span class="tex-span"><i>m</i></span> holes on it. More precisely, cup <span class="tex-span"><i>i</i></span> is on the table at the position <span class="tex-span"><i>x</i> = <i>i</i></span>.</p><p>The problematic bone is initially at the position <span class="tex-span"><i>x</i> = 1</span>. Zane will confuse the audience by swapping the cups <span class="tex-span"><i>k</i></span> times, the <span class="tex-span"><i>i</i></span>-th time of which involves the cups at the positions <span class="tex-span"><i>x</i> = <i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>x</i> = <i>v</i><sub class="lower-index"><i>i</i></sub></span>. If the bone happens to be at the position where there is a hole at any time, it will fall into the hole onto the ground and will not be affected by future swapping operations.</p><p>Do not forget that Zane is a wizard. When he swaps the cups, he does not move them ordinarily. Instead, he teleports the cups (along with the bone, if it is inside) to the intended positions. Therefore, for example, when he swaps the cup at <span class="tex-span"><i>x</i> = 4</span> and the one at <span class="tex-span"><i>x</i> = 6</span>, they will not be at the position <span class="tex-span"><i>x</i> = 5</span> at any moment during the operation.</p><center> <img class="tex-graphics" src="file://2dwlI3RY.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Zane’s puppy, Inzane, is in trouble. Zane is away on his vacation, and Inzane cannot find his beloved bone, as it would be too exhausting to try opening all the cups. Inzane knows that the Codeforces community has successfully helped Zane, so he wants to see if it could help him solve his problem too. Help Inzane determine the final position of the bone.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 3·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of cups, the number of holes on the table, and the number of swapping operations, respectively.</p><p>The second line contains <span class="tex-span"><i>m</i></span> <span class="tex-font-style-bf">distinct</span> integers <span class="tex-span"><i>h</i><sub class="lower-index">1</sub>, <i>h</i><sub class="lower-index">2</sub>, ..., <i>h</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— the positions along the <span class="tex-span"><i>x</i></span>-axis where there is a hole on the table.</p><p>Each of the next <span class="tex-span"><i>k</i></span> lines contains two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub></span>)&nbsp;— the positions of the cups to be swapped.</p></div><div class="output-specification"><p>Print one integer&nbsp;— the final position along the <span class="tex-span"><i>x</i></span>-axis of the bone.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 3·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of cups, the number of holes on the table, and the number of swapping operations, respectively.</p><p>The second line contains <span class="tex-span"><i>m</i></span> <span class="tex-font-style-bf">distinct</span> integers <span class="tex-span"><i>h</i><sub class="lower-index">1</sub>, <i>h</i><sub class="lower-index">2</sub>, ..., <i>h</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— the positions along the <span class="tex-span"><i>x</i></span>-axis where there is a hole on the table.</p><p>Each of the next <span class="tex-span"><i>k</i></span> lines contains two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub></span>)&nbsp;— the positions of the cups to be swapped.</p>

## Output

<p>Print one integer&nbsp;— the final position along the <span class="tex-span"><i>x</i></span>-axis of the bone.</p>





```input1
7 3 4
3 4 6
1 2
2 5
5 7
7 1

```




```input2
5 1 2
2
1 2
2 4

```




```output1
1
```




```output2
2
```



## Note

<p>In the first sample, after the operations, the bone becomes at <span class="tex-span"><i>x</i> = 2</span>, <span class="tex-span"><i>x</i> = 5</span>, <span class="tex-span"><i>x</i> = 7</span>, and <span class="tex-span"><i>x</i> = 1</span>, respectively.</p><p>In the second sample, after the first operation, the bone becomes at <span class="tex-span"><i>x</i> = 2</span>, and falls into the hole onto the ground.</p>
