## Description

<div><p>Vanya smashes potato in a vertical food processor. At each moment of time the height of the potato in the processor doesn't exceed <span class="tex-span"><i>h</i></span> and the processor smashes <span class="tex-span"><i>k</i></span> centimeters of potato each second. If there are less than <span class="tex-span"><i>k</i></span> centimeters remaining, than during this second processor smashes all the remaining potato.</p><p>Vanya has <span class="tex-span"><i>n</i></span> pieces of potato, the height of the <span class="tex-span"><i>i</i></span>-th piece is equal to <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. He puts them in the food processor one by one starting from the piece number <span class="tex-span">1</span> and finishing with piece number <span class="tex-span"><i>n</i></span>. Formally, each second the following happens:</p><ol> <li> If there is at least one piece of potato remaining, Vanya puts them in the processor one by one, until there is not enough space for the next piece. </li><li> Processor smashes <span class="tex-span"><i>k</i></span> centimeters of potato (or just everything that is inside). </li></ol><p>Provided the information about the parameter of the food processor and the size of each potato in a row, compute how long will it take for all the potato to become smashed.</p></div><div class="input-specification"><p>The first line of the input contains integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>h</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000, 1 ≤ <i>k</i> ≤ <i>h</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of pieces of potato, the height of the food processor and the amount of potato being smashed each second, respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>h</i></span>)&nbsp;— the heights of the pieces.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the number of seconds required to smash all the potatoes following the process described in the problem statement.</p></div>

## Input

<p>The first line of the input contains integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>h</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000, 1 ≤ <i>k</i> ≤ <i>h</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of pieces of potato, the height of the food processor and the amount of potato being smashed each second, respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>h</i></span>)&nbsp;— the heights of the pieces.</p>

## Output

<p>Print a single integer&nbsp;— the number of seconds required to smash all the potatoes following the process described in the problem statement.</p>





```input1
5 6 3
5 4 3 2 1

```




```input2
5 6 3
5 5 5 5 5

```




```input3
5 6 3
1 2 1 1 1

```




```output1
5

```




```output2
10

```




```output3
2

```



## Note

<p>Consider the first sample. </p><ol> <li> First Vanya puts the piece of potato of height <span class="tex-span">5</span> into processor. At the end of the second there is only amount of height <span class="tex-span">2</span> remaining inside. </li><li> Now Vanya puts the piece of potato of height <span class="tex-span">4</span>. At the end of the second there is amount of height <span class="tex-span">3</span> remaining. </li><li> Vanya puts the piece of height <span class="tex-span">3</span> inside and again there are only <span class="tex-span">3</span> centimeters remaining at the end of this second. </li><li> Vanya finally puts the pieces of height <span class="tex-span">2</span> and <span class="tex-span">1</span> inside. At the end of the second the height of potato in the processor is equal to <span class="tex-span">3</span>. </li><li> During this second processor finally smashes all the remaining potato and the process finishes. </li></ol><p>In the second sample, Vanya puts the piece of height <span class="tex-span">5</span> inside and waits for <span class="tex-span">2</span> seconds while it is completely smashed. Then he repeats the same process for <span class="tex-span">4</span> other pieces. The total time is equal to <span class="tex-span">2·5 = 10</span> seconds.</p><p>In the third sample, Vanya simply puts all the potato inside the processor and waits <span class="tex-span">2</span> seconds.</p>
