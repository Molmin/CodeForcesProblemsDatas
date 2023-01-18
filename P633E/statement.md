## Description

<div><p>An e-commerce startup pitches to the investors to get funding. They have been functional for <span class="tex-span"><i>n</i></span> weeks now and also have a website!</p><p>For each week they know the number of unique visitors during this week <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and the revenue <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>. To evaluate the potential of the startup at some range of weeks from <span class="tex-span"><i>l</i></span> to <span class="tex-span"><i>r</i></span> inclusive investors use the minimum among the maximum number of visitors multiplied by <span class="tex-span">100</span> and the minimum revenue during this period, that is: </p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://V58ZsuHE.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>The truth is that investors have no idea how to efficiently evaluate the startup, so they are going to pick some <span class="tex-span"><i>k</i></span> random distinct weeks <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and give them to managers of the startup. For each <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> they should pick some <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub> ≥ <i>l</i><sub class="lower-index"><i>i</i></sub></span> and report maximum number of visitors and minimum revenue during this period.</p><p>Then, investors will calculate the potential of the startup for each of these ranges and take minimum value of <span class="tex-span"><i>p</i>(<i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>)</span> as the total evaluation grade of the startup. Assuming that managers of the startup always report the optimal values of <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> for some particular <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, i.e., the value such that the resulting grade of the startup is maximized, what is the expected resulting grade of the startup? </p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 1 000 000</span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">7</sup></span>)&nbsp;— the number of unique visitors during each week.</p><p>The third line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">7</sup></span>)&nbsp;—the revenue for each week.</p></div><div class="output-specification"><p>Print a single real value&nbsp;— the expected grade of the startup. Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. </p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct, if <img align="middle" class="tex-formula" src="file://0kZAMuqk.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 1 000 000</span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">7</sup></span>)&nbsp;— the number of unique visitors during each week.</p><p>The third line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">7</sup></span>)&nbsp;—the revenue for each week.</p>

## Output

<p>Print a single real value&nbsp;— the expected grade of the startup. Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. </p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct, if <img align="middle" class="tex-formula" src="file://0kZAMuqk.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
3 2
3 2 1
300 200 300

```




```output1
133.3333333

```



## Note

<p>Consider the first sample.</p><p>If the investors ask for <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub> = 1</span> onwards, startup will choose <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub> = 1</span>, such that max number of visitors is <span class="tex-span">3</span> and minimum revenue is <span class="tex-span">300</span>. Thus, potential in this case is <span class="tex-span"><i>min</i>(3·100, 300) = 300</span>.</p><p>If the investors ask for <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub> = 2</span> onwards, startup will choose <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub> = 3</span>, such that max number of visitors is <span class="tex-span">2</span> and minimum revenue is <span class="tex-span">200</span>. Thus, potential in this case is <span class="tex-span"><i>min</i>(2·100, 200) = 200</span>.</p><p>If the investors ask for <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub> = 3</span> onwards, startup will choose <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub> = 3</span>, such that max number of visitors is <span class="tex-span">1</span> and minimum revenue is <span class="tex-span">300</span>. Thus, potential in this case is <span class="tex-span"><i>min</i>(1·100, 300) = 100</span>.</p><p>We have to choose a set of size <span class="tex-span">2</span> equi-probably and take minimum of each. The possible sets here are : <span class="tex-span">{200, 300}</span>,<span class="tex-span">{100, 300}</span>,<span class="tex-span">{100, 200}</span>, effectively the set of possible values as perceived by investors equi-probably: <span class="tex-span">{200, 100, 100}</span>. Thus, the expected value is <span class="tex-span">(100 + 200 + 100) / 3 = 133.(3)</span>.</p>
